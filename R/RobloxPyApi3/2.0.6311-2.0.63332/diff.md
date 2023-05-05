# Comparing `tmp/RobloxPyApi3-2.0.6311.tar.gz` & `tmp/RobloxPyApi3-2.0.63332.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobloxPyApi3-2.0.6311.tar", last modified: Fri May  5 19:02:29 2023, max compression
+gzip compressed data, was "RobloxPyApi3-2.0.63332.tar", last modified: Fri May  5 19:18:47 2023, max compression
```

## Comparing `RobloxPyApi3-2.0.6311.tar` & `RobloxPyApi3-2.0.63332.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 19:02:29.016200 RobloxPyApi3-2.0.6311/
--rw-rw-rw-   0        0        0       61 2023-04-27 12:20:20.000000 RobloxPyApi3-2.0.6311/MANIFEST.in
--rw-rw-rw-   0        0        0     2228 2023-05-05 19:02:29.015199 RobloxPyApi3-2.0.6311/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-05 19:02:28.991018 RobloxPyApi3-2.0.6311/RobloxPyApi3/
--rw-rw-rw-   0        0        0    20159 2023-04-28 09:51:23.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/AccountInformation.py
--rw-rw-rw-   0        0        0    15233 2023-04-09 12:42:10.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/Auth.py
--rw-rw-rw-   0        0        0    21919 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/Avatar.py
--rw-rw-rw-   0        0        0    16576 2023-04-27 13:25:52.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/Captcha.py
--rw-rw-rw-   0        0        0    36825 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/Catalog.py
--rw-rw-rw-   0        0        0     2739 2023-04-08 19:22:28.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/Check.png
--rw-rw-rw-   0        0        0    18452 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/Client.py
--rw-rw-rw-   0        0        0     1557 2023-04-12 19:25:10.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/Enums.py
--rw-rw-rw-   0        0        0     2213 2023-04-09 08:16:10.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/Errors.py
--rw-rw-rw-   0        0        0    14748 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/FriendsAPI.py
--rw-rw-rw-   0        0        0     5938 2023-04-27 12:30:26.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/JoinGame.py
--rw-rw-rw-   0        0        0      461 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/LeaveGame.py
--rw-rw-rw-   0        0        0    11364 2023-04-28 09:51:46.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/MultiAccount.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:02:29.015199 RobloxPyApi3-2.0.6311/RobloxPyApi3/Place/
--rw-rw-rw-   0        0        0     1977 2023-03-30 08:25:08.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/Place/CallMethods.py
--rw-rw-rw-   0        0        0     3312 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/Place/Instructions.py
--rw-rw-rw-   0        0        0    26891 2023-04-28 07:41:46.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/Place/Place.py
--rw-rw-rw-   0        0        0      122 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/Place/__init__.py
--rw-rw-rw-   0        0        0     9691 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/Place/rbxLua2py.py
--rw-rw-rw-   0        0        0     5550 2023-03-03 16:26:02.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/Place.py
--rw-rw-rw-   0        0        0        0 2023-03-03 14:18:04.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/PlacePropTypes.py
--rw-rw-rw-   0        0        0      505 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/SessionUtilities.py
--rw-rw-rw-   0        0        0       50 2023-04-15 15:18:22.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/Test.py
--rw-rw-rw-   0        0        0     3614 2023-04-28 08:41:48.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/Utilities.py
--rw-rw-rw-   0        0        0     1594 2023-04-27 13:25:52.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/Version.py
--rw-rw-rw-   0        0        0     2498 2023-04-27 13:25:52.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/__Changes__.py
--rw-rw-rw-   0        0        0    50881 2023-04-27 12:22:44.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/__init__.py
--rw-rw-rw-   0        0        0     4637 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3/friends.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:02:29.010876 RobloxPyApi3-2.0.6311/RobloxPyApi3.egg-info/
--rw-rw-rw-   0        0        0     2228 2023-05-05 19:02:28.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-05-05 19:02:28.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 19:02:28.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-05 19:02:28.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-05 19:02:28.000000 RobloxPyApi3-2.0.6311/RobloxPyApi3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 19:02:29.016200 RobloxPyApi3-2.0.6311/setup.cfg
--rw-rw-rw-   0        0        0     2717 2023-05-05 19:02:22.000000 RobloxPyApi3-2.0.6311/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:18:48.000000 RobloxPyApi3-2.0.63332/
+-rw-rw-rw-   0        0        0       61 2023-04-27 12:20:20.000000 RobloxPyApi3-2.0.63332/MANIFEST.in
+-rw-rw-rw-   0        0        0     2229 2023-05-05 19:18:48.000000 RobloxPyApi3-2.0.63332/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-05 19:18:48.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/
+-rw-rw-rw-   0        0        0    19220 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/AccountInformation.py
+-rw-rw-rw-   0        0        0    15348 2023-05-05 19:16:44.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/Auth.py
+-rw-rw-rw-   0        0        0    21919 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/Avatar.py
+-rw-rw-rw-   0        0        0    16278 2023-05-05 18:11:54.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/Captcha.py
+-rw-rw-rw-   0        0        0    36825 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/Catalog.py
+-rw-rw-rw-   0        0        0     2739 2023-04-08 19:22:28.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/Check.png
+-rw-rw-rw-   0        0        0    18452 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/Client.py
+-rw-rw-rw-   0        0        0     1557 2023-04-12 19:25:10.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/Enums.py
+-rw-rw-rw-   0        0        0     2213 2023-04-09 08:16:10.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/Errors.py
+-rw-rw-rw-   0        0        0    14748 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/FriendsAPI.py
+-rw-rw-rw-   0        0        0     5938 2023-04-27 12:30:26.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/JoinGame.py
+-rw-rw-rw-   0        0        0      461 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/LeaveGame.py
+-rw-rw-rw-   0        0        0     9576 2023-05-05 19:16:44.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/MultiAccount.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:18:48.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/Place/
+-rw-rw-rw-   0        0        0     1977 2023-03-30 08:25:08.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/Place/CallMethods.py
+-rw-rw-rw-   0        0        0     3312 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/Place/Instructions.py
+-rw-rw-rw-   0        0        0    26394 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/Place/Place.py
+-rw-rw-rw-   0        0        0      122 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/Place/__init__.py
+-rw-rw-rw-   0        0        0     9691 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/Place/rbxLua2py.py
+-rw-rw-rw-   0        0        0     5550 2023-03-03 16:26:02.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/Place.py
+-rw-rw-rw-   0        0        0        0 2023-03-03 14:18:04.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/PlacePropTypes.py
+-rw-rw-rw-   0        0        0      505 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/SessionUtilities.py
+-rw-rw-rw-   0        0        0       50 2023-04-15 15:18:22.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/Test.py
+-rw-rw-rw-   0        0        0     2762 2023-04-27 12:24:10.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/Utilities.py
+-rw-rw-rw-   0        0        0     1594 2023-04-27 13:26:04.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/Version.py
+-rw-rw-rw-   0        0        0     1049 2023-05-05 11:47:44.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/__Changes__.py
+-rw-rw-rw-   0        0        0    50881 2023-04-27 12:22:44.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/__init__.py
+-rw-rw-rw-   0        0        0     4637 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3/friends.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:18:48.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3.egg-info/
+-rw-rw-rw-   0        0        0     2229 2023-05-05 19:18:48.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-05-05 19:18:48.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 19:18:48.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-05 19:18:48.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-05 19:18:48.000000 RobloxPyApi3-2.0.63332/RobloxPyApi3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 19:18:48.000000 RobloxPyApi3-2.0.63332/setup.cfg
+-rw-rw-rw-   0        0        0     2718 2023-05-05 19:17:44.000000 RobloxPyApi3-2.0.63332/setup.py
```

### Comparing `RobloxPyApi3-2.0.6311/PKG-INFO` & `RobloxPyApi3-2.0.63332/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobloxPyApi3
-Version: 2.0.6311
+Version: 2.0.63332
 Summary: RobloxPyApi3 is a Python API controller for Roblox, offering API wrapping, multi-account management, and more. Create and manage Roblox accounts and Places with ease.
 Author: pyProjects3 (github.com/pyProjects3)
 License: MIT
 Keywords: Roblox,Api,wrapper,Bot,Client,Automated,Account Management,rbx,Python3,Place automation,post requests,get requests,JSON,Authorization,Roblox Development
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/AccountInformation.py` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/AccountInformation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import random
 
 import requests
 from RobloxPyApi3.Utilities import Delete_Request as __Delete_Request__
 from RobloxPyApi3.Utilities import Post_Request as __Post_Request__
-from RobloxPyApi3.Utilities import Post_Request2 as __p2
 from RobloxPyApi3.Utilities import Get_Request as __Get_Request__
 from RobloxPyApi3.Enums import MonthsNum as Months
 import RobloxPyApi3.Errors as Errors
 from RobloxPyApi3.Auth import Gender
 from RobloxPyApi3.Enums import Privacy
 import warnings
 from RobloxPyApi3.Auth import NewDate as Date
@@ -16,15 +15,15 @@
         self.CCode: int = CountryCode
         self.perfix: int = Perfix
         self.Phone: int = phone
 
 
 def SetDescription(session,description,showErrors = True) -> requests.Response:
     try:
-        req = __p2("https://accountinformation.roblox.com/v1/description",
+        req = __Post_Request__("https://accountinformation.roblox.com/v1/description",
                                session=session,
                                data={
                                    "description":description
                                })
         if req.status_code != 200:
 
             if 'errors' in req.json() and showErrors:
@@ -59,14 +58,15 @@
 
     try:
         req = __Get_Request__("https://accountinformation.roblox.com/v1/birthdate",
                                session=session)
         if req.status_code != 200:
 
             if 'errors' in req.json() and showErrors:
+                print(req.json())
                 raise Errors.APIError(f"(response:{req.status_code}) {req.json()['errors'][0]['message']}")
 
         return req
     except Exception as error:
         if showErrors:
             raise Errors.MakeRequestFailed("An error occurred: {}".format(error))
 def SetPhone(session,password,Phone:PhoneNumber,showErrors = True) -> requests.Response:
@@ -352,50 +352,26 @@
             if 'errors' in req.json() and showErrors:
                 raise Errors.APIError(f"(response:{req.status_code}) {req.json()['errors'][0]['message']}")
 
         return req
     except Exception as error:
         if showErrors:
             raise Errors.MakeRequestFailed("An error occurred: {}".format(error))
-def GetDescription(session,showErrors = True) -> requests.Response:
-    try:
-        req = __Get_Request__(f"https://accountinformation.roblox.com/v1/description",
-                               session=session)
-        if req.status_code != 200:
-
-            if 'errors' in req.json() and showErrors:
-                raise Errors.APIError(f"(response:{req.status_code}) {req.json()['errors'][0]['message']}")
-
-        return req
-    except Exception as error:
-        if showErrors:
-            raise Errors.MakeRequestFailed("An error occurred: {}".format(error))
 class AccountInformationSession(object):
     def __init__(self,session,password):
         self.Session = session
         self.Password = password
-
-    def GetDescription(self,showErrors = True):
-        return GetBirthdate(session=self.Session, showErrors=showErrors)
     def SetDescription(self,Description,showErrors = True) -> requests.Response:
         return SetDescription(session=self.Session,description=Description,showErrors=showErrors)
     def SetGender(self,gender:Gender,showErrors = True) -> requests.Response:
         return SetGender(session=self.Session,gender=gender,showErrors=showErrors)
     def GetBirthDate(self,showErrors = True) -> requests.Response:
         return GetBirthdate(session=self.Session, showErrors=showErrors)
-    def GetGender(self,showErrors = True) -> Gender:
-        req = GetGender(session=self.Session,showErrors = showErrors)
-        gen = req.json()['gender']
-        if gen == 2:
-            res = Gender.male
-        elif gen == 1:
-            res = Gender.female
-        else:
-            res = Gender.Unknown
-        return res
+    def GetGender(self,showErrors = True):
+        return GetGender(session=self.Session,showErrors = showErrors)
     def SetBirthdate(self,Date:Date,showErrors = True):
         warnings.warn("This function is deprecated. This feature now requires a Challange so it will probably break.")
         return SetBirthdate(session=self.Session,NewDate=Date,Password=self.Password,showErrors=showErrors)
     def Get_Xbox_Consecutive_login_days(self,showErrors = True):
         return Get_Xbox_Consecutive_login_days(session=self.Session,showErrors = showErrors)
 
     def Get_Metatable(self, showErrors=True):
```

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/Auth.py` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/Auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import random
-from Enums import Months
-from Enums import Gender
-from Enums import CaptchaMetatable
-from Captcha import Captcha,SessionCaptcha
-from Enums import MonthsNum
+from RobloxPyApi3.Enums import Months
+from RobloxPyApi3.Enums import Gender
+from RobloxPyApi3.Enums import CaptchaMetatable
+from RobloxPyApi3.Captcha import SessionCaptcha
+from RobloxPyApi3.Enums import MonthsNum
 import string
 import requests
 class Date:
     def __init__(self,day,month,Year):
         self.d: int = day
         self.year: int = Year
         self.month = month.value
@@ -214,19 +214,20 @@
 
         def MakePost():
             tok =  session.post(
                                      'https://auth.roblox.com/v1/usernames/validate'
                                  ).headers['x-csrf-token']
             Debug(tok)
             post = session.post("https://auth.roblox.com/v2/signup",
-                                 headers={"Accept": "application/json", "x-csrf-token":tok}, json=JSONSignup)
+                                 headers={"Content-Type":"application/json","Accept": "application/json", "x-csrf-token":tok}, json=JSONSignup)
+            print(post.json())
             return post
 
         a = MakePost()
-        b = a.json()['failureDetails'][0]['fieldData']
+        b = a.headers['rblx-challenge-metadata']
         if b:
             Output("Captcha is required!")
             td = c.GetDetailsFromFieldData(b)
             f = c.StartSessionFromDetails(td['TokenID'], td['location'])
             Debug(f.json())
             if f:
                 # make the authenticated request using the session of the current user
@@ -295,15 +296,15 @@
                             headers={"Accept": "application/json", "x-csrf-token": tok}, json=JSONLogin)
         return post
 
     a = MakePost()
     b = a.json()['errors'][0]['fieldData']
     if b:
         Output("Captcha is required!")
-        td = c.GetDetailsFromFieldData2(b)
+        td = c.GetDetailsFromFieldData(b)
         f = c.StartSessionFromDetails(td['TokenID'], td['location'])
         Debug(f.json())
         if "user" in f.json():
             # make the authenticated request using the session of the current user
             Output("Success")
             return session, {"Username": Username, 'Password': password, "UserId": f.json()["user"]['id'],"displayName": f.json()["user"]['displayName']}
         else:
@@ -341,15 +342,15 @@
                                 headers={"Accept": "application/json", "x-csrf-token": tok}, json=JSONLogin)
             return post
 
         a = MakePost()
         b = a.json()['errors'][0]['fieldData']
         if b:
             Output("Captcha is required!")
-            td = c.GetDetailsFromFieldData2(b)
+            td = c.GetDetailsFromFieldData(b)
             f = c.StartSessionFromDetails(td['TokenID'], td['location'])
             Debug(f.json())
             if f:
                 # make the authenticated request using the session of the current user
                 # make the authenticated request using the session of the current user
                 if "user" in f.json():
                     # make the authenticated request using the session of the current user
```

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/Avatar.py` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/Avatar.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/Captcha.py` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/Captcha.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import requests
 import random
 import time
 import webbrowser as WEB
 import pyautogui
+import base64
+import json
 class Captcha:
     def __init__(self,CaptchaRequiredRobloxAPI,data,Headers,WaitAfterComplete = 4.5,CaptchaType = "A2A14B1D-1AF3-C791-9BBC-EE33CC7A0A6F"):
         self.URL = CaptchaRequiredRobloxAPI
         self.Token = None
         self.ID = None
         self.blob = None
         self.TokenID = None
@@ -17,14 +19,15 @@
         self.Type: str = CaptchaType
         self.Headers = Headers
         self.AccessToken = requests.post(
                             'https://auth.roblox.com/v1/usernames/validate'
                         ).headers['x-csrf-token']
     def MakePost(self):
         post = requests.post(self.URL, headers=self.Headers, json=self.data)
+
         return post
     def GetDetailsFromFieldData(self,fieldData):
         try:
 
             _details_ = fieldData.split(',')
             self.ID = _details_[0]
             self.blob = _details_[1]
@@ -91,51 +94,14 @@
                 self.StartSession()
                 return self.Token
             else:
                 print("Failed to get captcha TOKEN")
         except Exception as error:
             print(error)
             return error
-    def GetDetailsFromFieldData2(self,fieldData):
-        try:
-
-
-            self.ID = fieldData.split('\",\"unifiedCaptchaId\":\"')[1].split('\"}"}]')[0].split('"}')[0]
-            self.blob = fieldData.split('"{\"dxBlob\":\"')[0].split('\",')[0].split('{"dxBlob":"')[1]
-            if self.ID:
-                pass
-            else:
-                print("Failed to get captcha ID.")
-            if self.blob:
-                pass
-            else:
-                print("Failed to get captcha BLOB")
-            tokpostreq = requests.post(
-                f'https://roblox-api.arkoselabs.com/fc/gt2/public_key/{self.Type}',
-
-                data={
-                    'public_key': self.Type,
-                    'userbrowser': "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/95.0.4638.54 Safari/537.36 Edg/95.0.1020.30",
-                    'rnd': f'0.{random.randint(1000, 10000000)}',
-                    'data[blob]': self.blob,
-                    'language': 'en'
-                }
-            )
-            tokpost = tokpostreq.json()['token']
-            if tokpost:
-                self.Token = tokpost
-                self.TokenDetails = self.Token.split('|')
-                self.TokenID = self.TokenDetails[0]
-                self.location = self.TokenDetails[1]
-                return {"Token":self.Token,"TokenID":self.TokenDetails[0],'location':self.TokenDetails[1],"blob":self.blob,'id':self.ID}
-            else:
-                print("Failed to get captcha TOKEN")
-        except Exception as error:
-            print(error)
-            return error
     def StartSession(self):
         global t
         if self.TokenDetails:
             solver_url = f'https://roblox-api.arkoselabs.com/fc/gc/?token={self.TokenID}&{self.location}&lang=en&pk=A2A14B1D-1AF3-C791-9BBC-EE33CC7A0A6F&cdn_url=https%3A%2F%2Froblox-api.arkoselabs.com%2Fcdn%2Ffc'
             #print(
                 #f'- Received Captcha Details!\n\n\nCaptchaId : {self.ID}\nCaptchaBlob : {self.blob}\nLocation : {self.location}\ntoken : {self.TokenID}\n\n\n(Starting selenium browser to solve the captcha)..\n\n\n')
             print("[INFO] Starting Web browser to solve the captcha.")
@@ -192,50 +158,67 @@
         self.data: dict = data
         self.Headers = Headers
         self.AccessToken = requests.post(
                             'https://auth.roblox.com/v1/usernames/validate'
                         ).headers['x-csrf-token']
     def MakePost(self):
         post = self.session.post(self.URL, headers=self.Headers, json=self.data)
+
         return post
     def GetDetailsFromFieldData(self,fieldData):
         try:
 
-            _details_ = fieldData.split(',')
-            self.ID = _details_[0]
-            self.blob = _details_[1]
+            _details_ = json.loads(base64.b64decode(fieldData).decode('utf-8'))
+            print(_details_)
+            self.ID = _details_['unifiedCaptchaId'].split('"}')[0]
+            self.blob = _details_["dataExchangeBlob"].split('","')[0]
+
+            print(self.blob,self.ID)
+            if _details_:
+                print(_details_)
+                print(self.blob)
+                pass
+
+            else:
+                print("Cant")
+                self.ID = _details_[0]
+                self.blob = _details_[1]
+
             if self.ID:
                 pass
             else:
                 print("Failed to get captcha ID.")
             if self.blob:
                 pass
             else:
                 print("Failed to get captcha BLOB")
-            tokpost = self.session.post(
+            print(self.blob,self.ID)
+            tokpost = requests.post(
                 f'https://roblox-api.arkoselabs.com/fc/gt2/public_key/{self.Type}',
 
                 data={
                     'public_key': self.Type,
                     'userbrowser': "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/95.0.4638.54 Safari/537.36 Edg/95.0.1020.30",
                     'rnd': f'0.{random.randint(1000, 10000000)}',
                     'data[blob]': self.blob,
                     'language': 'en'
                 }
-            ).json()['token']
+            ).json()["token"]
+            print(self.blob)
+
             if tokpost:
                 self.Token = tokpost
                 self.TokenDetails = self.Token.split('|')
                 self.TokenID = self.TokenDetails[0]
                 self.location = self.TokenDetails[1]
                 return {"Token":self.Token,"TokenID":self.TokenDetails[0],'location':self.TokenDetails[1],"blob":self.blob,'id':self.ID}
             else:
                 print("Failed to get captcha TOKEN")
         except Exception as error:
-            print(error)
+            print(error) #eyJjYXB0Y2hhVG9rZW4iOiIiLCAidW5pZmllZENhcHRjaGFJZCI6InpnZWFBWkJ0QzhNZlgzRlVGa0gyamoiLCAiZGF0YUV4Y2hhbmdlQmxvYiI6IkYxeEFhNDlaQllQOU9Cai8uTExVdzFNM2FqM0tiTnJZV2VRdjRIZG5YaVo4RUIxNjg1Y3R4YTd3cXpiUSt6dis4NlAvTEJYb3JjQnA2cFY5Uzl2UW5JbXF1eTZMektIdm8zbERodWZibERuN0VVdS9tNEt4aElJcWt5L2JKMDlaWkxtc3l1dXo4eE5jL093cXB1bDNjWDhWRmZ0UGhFUU9SYnVGenVUTzZvN1ZmWlZUVHdHT3BtUVFuaDZSellnNUN1bHgrT0grU1ZOVUlBUHFwVXlLYXBnVlFSdVY3eWd6MXZHNnV5YUpTWGl6cU8xUWd5czRpWkZPcDMzMWJqa2ZZL1IzaUY0STF0dUlreUNNR01CU3Izd3NNRlpsZEZSQzJWWFY4dmEyaHhpRmhiWG9EWHU2NjIyWUl2d2RPTTcwRzlGL1VPTTNRNlprS2l0T3JYdnZ2bE03YWNxSjlnQ1pnTWl5ZjBmOW5jS1Rvcm9SVFV1NUFXMkp1dXNDdVJ5aTM4Z3lkdHlwTW9QajdVS2U3K1BiSG5Wa0U3VkM1QlQvMzJqaERFdmNnZEtMUm1ORVVlVHdZOXVGYlpnPT0iLCAiYWN0aW9uVHlwZSI6IlNpZ251cCIsICJyZXF1ZXN0UGF0aCI6Ii92Mi9zaWdudXAiLCAicmVxdWVzdE1ldGhvZCI6IlBPU1QifQ
             return error
     def GetDetailsFromFieldData2(self,fieldData):
         try:
 
 
             self.ID = fieldData.split('\",\"unifiedCaptchaId\":\"')[1].split('\"}"}]')[0].split('"}')[0]
             self.blob = fieldData.split('"{\"dxBlob\":\"')[0].split('\",')[0].split('{"dxBlob":"')[1]
@@ -243,15 +226,15 @@
                 pass
             else:
                 print("Failed to get captcha ID.")
             if self.blob:
                 pass
             else:
                 print("Failed to get captcha BLOB")
-            tokpostreq = self.session.post(
+            tokpostreq = requests.post(
                 f'https://roblox-api.arkoselabs.com/fc/gt2/public_key/{self.Type}',
 
                 data={
                     'public_key': self.Type,
                     'userbrowser': "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/95.0.4638.54 Safari/537.36 Edg/95.0.1020.30",
                     'rnd': f'0.{random.randint(1000, 10000000)}',
                     'data[blob]': self.blob,
@@ -268,16 +251,17 @@
             else:
                 print("Failed to get captcha TOKEN")
         except Exception as error:
             print(error)
             return error
     def GetDetails(self):
         try:
-
-            _details_ = self.MakePost().json()["failureDetails"][0]["fieldData"].split(',')
+            _p = self.MakePost().json()
+            print(_p)
+            _details_ = _p["failureDetails"][0]["fieldData"].split(',')
             self.ID = _details_[0]
             self.blob = _details_[1]
             if self.ID:
                 pass
             else:
                 print("Failed to get captcha ID.")
             if self.blob:
@@ -305,16 +289,16 @@
             else:
                 print("Failed to get captcha TOKEN")
         except Exception as error:
             print(error)
             return error
     def StartSession(self):
         global t
-        if self.TokenDetails:
-            solver_url = f'https://roblox-api.arkoselabs.com/fc/gc/?token={self.TokenID}&{self.location}&lang=en&pk=A2A14B1D-1AF3-C791-9BBC-EE33CC7A0A6F&cdn_url=https%3A%2F%2Froblox-api.arkoselabs.com%2Fcdn%2Ffc'
+        if self.TokenDetails: # :(
+            solver_url = f'https://roblox-api.arkoselabs.com/fc/gc/?token={self.TokenID}&{self.location}&lang=en&pk={self.Type}&cdn_url=https%3A%2F%2Froblox-api.arkoselabs.com%2Fcdn%2Ffc'
             #print(
                 #f'- Received Captcha Details!\n\n\nCaptchaId : {self.ID}\nCaptchaBlob : {self.blob}\nLocation : {self.location}\ntoken : {self.TokenID}\n\n\n(Starting selenium browser to solve the captcha)..\n\n\n')
             print("[INFO] Starting Web browser to solve the captcha.")
             time.sleep(1)
             WEB.open(solver_url)
             time.sleep(1)
```

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/Catalog.py` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/Catalog.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/Check.png` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/Check.png`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/Client.py` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/Client.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/Enums.py` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/Enums.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/Errors.py` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/Errors.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/FriendsAPI.py` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/FriendsAPI.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/JoinGame.py` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/JoinGame.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/MultiAccount.py` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/MultiAccount.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,34 +9,34 @@
 from typing import List
 import string
 import time
 
 class Account(SessionAPI):
 
     def __init__(self,session,username,password,Birthdate,userId,Gender):
-
+        super().__init__(session=session,Password=password)
         self.Username: str = username
         self.Password = password
         self.Birthdate = Birthdate
         self.UserId : int = userId
-        self.CurrentGender = None
         self.Session:requests.Session = session
         self.Gender = Gender
-        super().__init__(session=session,Password=password)
     @property
     def session(self):
         return self.Session
     def SetProxy(self,ProxyServer,Protocol = "http"):
         prot = Protocol.lower()
         self.Session.proxies[prot] = str("{}://{}".format(prot,ProxyServer))
+        print(self.Session.proxies)
     def RemoveProxies(self):
         self.Session.proxies.clear()
         #self.Session.proxies = None
     def SetProxies(self,dict):
         self.Session.proxies = dict
+        print(self.Session.proxies)
     @property
     def Cookie(self):
         return self.Session.cookies.get(name=".ROBLOSECURITY")
     def to_dict(self) -> dict:
         return {'password':self.Password,'Birthdate': "{} {} {}".format(self.Birthdate.d,self.Birthdate.month,self.Birthdate.year),"UserId":self.UserId,"Gender":self.Gender}
 class MultiAccountHandler:
     def __init__(self):
@@ -48,34 +48,30 @@
         Auth.init(CaptchaDelay=CaptchaDelay,Output=Outputting,Debug=Debugging)
     def SignUp(self,Username,password,gender = Gender.Random,birthday = Date(22,Months.JANUARY,1980),WaitAfterCaptcha = 2,retry = True) -> Account:
         Session,Info = Auth.signupSession(Username=Username,password=password,gender=gender,birthday=birthday,WaitAfterCaptcha=WaitAfterCaptcha,retry=retry)
         if 'UserId' in Info:
             acc = Account(Session,Username,password,birthday,Info["UserId"],Info["Gender"])
             self.AddAccount(acc)
             return acc
-    def Login(self, Username, password, birthday=Date(22, Months.JANUARY, 1980),
+    def Login(self, Username, password, gender=Gender.Random, birthday=Date(22, Months.JANUARY, 1980),
                WaitAfterCaptcha=2, retry=True) -> Account:
         Session, Info = Auth.LoginSession(Username=Username, password=password,
                                            WaitAfterCaptcha=WaitAfterCaptcha, retry=retry)
         if 'UserId' in Info:
             acc = Account(Session, Username, password, birthday, Info["UserId"], Info["Gender"])
             self.AddAccount(acc)
             return acc
 
     def AddAccount(self, account: Account):
         if not self.AccountInClass(account.Username):
             self.Accounts.append(account)
             self.AccountsDetails[account.Username] = account.to_dict()
-    def Save(self,Name = "SavedMultiHandler",Where=None):
-        if Where:
-            with open(f'{Where}\\{Name}.pkl', 'wb') as f:
-                pickle.dump(self, f)
-        else:
-            with open(f'{Name}.pkl', 'wb') as f:
-                pickle.dump(self, f)
+    def Save(self,Name = "SavedMultiHandler"):
+        with open(f'{Name}.pkl', 'wb') as f:
+            pickle.dump(self, f)
     def GetAccount(self,Name) -> Account:
         if self.Accounts != []:
 
             for account in self.Accounts:
                 if account.Username.lower() == Name.lower():
                     return account
     def AccountInClass(self,Name) -> bool:
@@ -89,27 +85,20 @@
         if self.AccountInClass(AccountName):
             account = self.GetAccount(AccountName)
             del self.AccountsDetails[account.Username]
             self.Accounts.remove(account)
     def RemoveAccountObject(self,Account:Account):
         del self.AccountsDetails[Account.Username]
         self.Accounts.remove(Account)
-    def Load(self,Name="SavedMultiHandler",CustomPath=None):
+    def Load(self,Name="SavedMultiHandler"):
         try:
-            if CustomPath:
-                with open(f'{CustomPath}', 'rb') as f:
-                    Data: 'MultiAccountHandler' = pickle.load(f)
-                    self.Accounts = Data.Accounts
-                    self.AccountsDetails = Data.AccountsDetails
-            else:
-                with open(f'{Name}.pkl', 'rb') as f:
-                    Data: 'MultiAccountHandler' = pickle.load(f)
-                    self.Accounts = Data.Accounts
-                    self.AccountsDetails = Data.AccountsDetails
-
+            with open(f'{Name}.pkl', 'rb') as f:
+                Data: 'MultiAccountHandler' = pickle.load(f)
+                self.Accounts = Data.Accounts
+                self.AccountsDetails = Data.AccountsDetails
         except FileNotFoundError:
             raise FileNotFoundError(f"File 'SavedMultiHandler.pkl' was not found, Save the Multi-handler to fix it.")
 
     def UpdateAllAccounts(self):
         if self.Accounts:
             for acc in self.Accounts:
                 # Get updated account info
@@ -122,80 +111,60 @@
 
                 # Update the properties of the account instance
                 acc.Password = updated_account.Password
                 acc.Birthdate = updated_account.Birthdate
                 acc.UserId = updated_account.UserId
                 acc.Gender = updated_account.Gender
                 acc.Session = updated_account.session
-                acc.CurrentGender = updated_account.GetGender()
-                acc.StarcodeAffiliates = updated_account.Get_Current_Starcode().json()
-                acc.PromotionChannels = updated_account.Get_Promotion_Channels().json()
-                acc.promotionChannelsVisibilityPrivacy = acc.PromotionChannels['promotionChannelsVisibilityPrivacy']
-                acc.Twitter = acc.PromotionChannels['twitter']
-                acc.Twitch = acc.PromotionChannels['twitch']
-                acc.Facebook = acc.PromotionChannels["facebook"]
-                acc.guilded = acc.PromotionChannels['guilded']
-                acc.CurrentBirthdate = updated_account.GetBirthDate()
-                acc.Youtube = acc.PromotionChannels['youtube']
-                acc.CurrentGender = updated_account.GetGender()
-                acc.description = updated_account.GetDescription().json()
-def Load_Handler(Name = "SavedMultiHandler",CustomPath = None) -> MultiAccountHandler:
+def Load_Handler(Name = "SavedMultiHandler") -> MultiAccountHandler:
     try:
-        if CustomPath:
-            with open(f'{CustomPath}', 'rb') as f:
-                return pickle.load(f)
-        else:
-            with open(f'{Name}.pkl', 'rb') as f:
-                return pickle.load(f)
+        with open(f'{Name}.pkl', 'rb') as f:
+            return pickle.load(f)
     except FileNotFoundError:
         return
-def Get_Handler(Name = "SavedMultiHandler",CustomPath = None):
+def Get_Handler(Name = "SavedMultiHandler"):
     try:
-        if CustomPath:
-            with open(f'{CustomPath}', 'rb') as f:
-                return f
-        else:
-            with open(f'{Name}.pkl', 'rb') as f:
-                return f
+        with open(f'{Name}.pkl', 'rb') as f:
+            return f
     except FileNotFoundError:
         return
-
+"""
 MAH = Load_Handler()
+print(MAH.AccountsDetails)
 try:
-    print(MAH.AccountsDetails)
     print()
-    # for i in range(2):
-    #   MAH.SignUp("".join(random.choices(string.digits + string.ascii_uppercase + string.ascii_lowercase,k=10)),"markdarss")
+    #for i in range(2):
+     #   MAH.SignUp("".join(random.choices(string.digits + string.ascii_uppercase + string.ascii_lowercase,k=10)),"markdarss")
     #    MAH.Save()
-    # for acc in MAH.Accounts:
+    #for acc in MAH.Accounts:
     #    rand = "".join(random.choices(string.hexdigits + string.whitespace + string.octdigits + string.punctuation + string.printable,k=200))
     #    print(acc.Username)
     #    continue
     # List of adjectives to use in the username
-    adjectives = ['Gamer', 'Cool', 'nice', 'green', 'red', 'Fearless', 'Dark', 'Bright', 'White', 'Shiny', "Good"]
+    adjectives = ['Gamer', 'Cool', 'nice', 'green', 'red', 'Fearless', 'Dark', 'Bright', 'White', 'Shiny',"Good"]
 
     # List of nouns to use in the username
     nouns = ['Wolf', 'Dragon', 'Knight', 'Warrior', 'Hero', 'Pirate', 'Ninja', 'Samurai', 'Wizard', 'Viking',
              "Emily", "Liam", "Ava", "Noah", "Olivia", "Ethan", "Emma", "Lucas", "Isabella", "Mason", "Sophia", "Logan",
              "Mia", "Jackson", "Charlotte", "Jacob", "Amelia", "Caden", "Harper", "William", "Evelyn", "Oliver",
              "Abigail", "Elijah", "Ella", "Grayson", "Madison", "Michael", "Scarlett", "Benjamin", "Avery", "Carter",
              "Lily", "Luke", "Chloe", "Daniel", "Aria", "Gabriel", "Ellie", "Matthew", "Nora", "Jayden", "Hazel",
              "James", "Zoe", "Lincoln", "Luna", "Jackson", "Grace", "Owen", "Violet", "Levi", "Riley", "Alexander",
              "Aurora", "Sebastian", "Aaliyah", "Isaac", "Stella", "Wyatt", "Nova", "Hunter", "Emilia", "Christian",
              "Everly", "Jonathan", "Valentina", "Ezra", "Adalyn", "Jaxon", "Brooklyn", "Nicholas", "Bella", "Jace",
              "Genesis", "Nathan", "Savannah", "Caleb", "Skylar", "Landon", "Paisley", "John", "Victoria", "David",
              "Eleanor", "Adam", "Leah", "Grayson", "Hannah", "Ian", "Audrey", "Cooper", "Aubrey", "Isaiah", "Claire",
              "Carson", "Penelope", "Charles", "Natalie", "Max", "Addison", "Joseph", "Mila", "Mateo", "Liliana",
-             "Antonio", "Rosalie", "User"]
-    # proxies = {
+             "Antonio", "Rosalie","User"]
+    #proxies = {
     #    'http': [
     #        "103.82.157.146:8080"
     #        "102.165.51.172:3128"
     #    ]
-    # }
+    #}
     proxies = {
         'http': [
             '182.18.208.59:3128',
             '103.127.1.130:80',
             '121.199.78.228:8888',
             '35.247.242.101:3129',
             '120.197.40.219:9002',
@@ -227,22 +196,18 @@
 
     # Combine a random adjective, noun, and number to create the username
     username = random.choice(adjectives) + random.choice(nouns) + str(number)
     print(username)
     # Print the generated username
     print(username)
     print(MAH.Accounts)
-    used = []
-    r = "".join(random.choices(string.digits + string.ascii_uppercase + string.ascii_lowercase, k=10))
+    r = "".join(random.choices(string.digits + string.ascii_uppercase + string.ascii_lowercase,k=10))
     MAH.UpdateAllAccounts()
-    for acc in MAH.Accounts:
-        print(acc.CurrentGender)
-    #print(MAH.Accounts[0].CurrentGender)
-        # acc.SetProxy(Protocol=prot,ProxyServer=procserv)
-    # for i in range(5):
-    # account = MAH.SignUp(username,"markdarss")
-    # if account:
-    # print(account.session)
-    # print(account.to_dict())
-except Exception as error:
-    print(error)
-    MAH.Save()
+    for i in range(5):
+        account = MAH.SignUp(username,"markdarss")
+        if account:
+            print(account.session)
+            print(account.to_dict())
+
+except Exception as err:
+    print(err)
+"""
```

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/Place/CallMethods.py` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/Place/CallMethods.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/Place/Instructions.py` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/Place/Instructions.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/Place/Place.py` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/Place/Place.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,28 +316,14 @@
     def CreateInstance(self):
         part = ET.SubElement(self.workspace, "Item")
         part.set("class", self.instance)
         part.set("referent", f"RBX{random.randint(100, 9999)}")
         self.CreatedInstance = part
         self.Props = ET.SubElement(part, "Properties")
         return self.root, self.workspace
-    def AddScript(self, Name, code):
-        inst = Script(self.Instance, self.root, Name)
-        inst.CreateInstance()
-        inst.CreatePropertiesSection()
-        inst.AddCode(code)
-        self.root = inst.root
-        return inst
-    def AddLocalScript(self, Name, code):
-        inst = LocalScript(self.Instance,self.root, Name)
-        inst.CreateInstance()
-        inst.CreatePropertiesSection()
-        inst.AddCode(code)
-        self.root = inst.root
-        return inst
 
     def CreatePropertiesSection(self):
         if not self.CreatedInstance:
             raise ValueError("CreateInstance method should be called first")
         self.Props = ET.SubElement(self.CreatedInstance, "Properties")
 
     def AddProperty(self, fullPropertyName, FullPropertyType, Value):
```

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/Place/rbxLua2py.py` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/Place/rbxLua2py.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/Place.py` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/Place.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/Utilities.py` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/Utilities.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,28 +9,14 @@
         tok = requests.post(
             'https://auth.roblox.com/v1/usernames/validate'
         ).headers['x-csrf-token']
     return tok
 def Post_Request(url, session = None, data=None) -> requests.Response:
     try:
         if session == None:
-            req = requests.post(url=url, data=data, headers={"Content-type":"application/json","accept": "application/json",
-                                                             "x-csrf-token": GetToken(),
-                                                             })
-            return req
-        else:
-            req = session.post(url=url, data=data, headers={"Content-type":"application/json","accept": "application/json",
-                                                            "x-csrf-token": GetToken(session),
-                                                            })
-            return req
-    except Exception as error:
-        raise Errors.MakeRequestFailed("An error occurred: {}".format(error))
-def Post_Request2(url, session = None, data=None) -> requests.Response:
-    try:
-        if session == None:
             req = requests.post(url=url, data=data, headers={"accept": "application/json",
                                                              "x-csrf-token": GetToken(),
                                                              })
             return req
         else:
             req = session.post(url=url, data=data, headers={"accept": "application/json",
                                                             "x-csrf-token": GetToken(session),
```

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/Version.py` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/Version.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/__init__.py` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/__init__.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3/friends.py` & `RobloxPyApi3-2.0.63332/RobloxPyApi3/friends.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3.egg-info/PKG-INFO` & `RobloxPyApi3-2.0.63332/RobloxPyApi3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobloxPyApi3
-Version: 2.0.6311
+Version: 2.0.63332
 Summary: RobloxPyApi3 is a Python API controller for Roblox, offering API wrapping, multi-account management, and more. Create and manage Roblox accounts and Places with ease.
 Author: pyProjects3 (github.com/pyProjects3)
 License: MIT
 Keywords: Roblox,Api,wrapper,Bot,Client,Automated,Account Management,rbx,Python3,Place automation,post requests,get requests,JSON,Authorization,Roblox Development
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `RobloxPyApi3-2.0.6311/RobloxPyApi3.egg-info/SOURCES.txt` & `RobloxPyApi3-2.0.63332/RobloxPyApi3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.6311/setup.py` & `RobloxPyApi3-2.0.63332/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 from RobloxPyApi3.Version import __Copyright__
-Version = "2.0.6311"
+Version = "2.0.63332"
 
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
-    install_requires=['requests','colorama','psutil','RobloxPyApi3Update',"Enums"],
+    install_requires=['requests','colorama','psutil','RobloxPyApi3Update','enums'],
     keywords=["Roblox","Api",'wrapper',"Bot",'Client','Automated',"Account Management","rbx","Python3","Place automation","post requests","get requests","JSON","Authorization","Roblox Development"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Microsoft :: Windows",
     ]
```

