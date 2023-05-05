# Comparing `tmp/fyers_apiv2-2.0.5.tar.gz` & `tmp/fyers_apiv2-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fyers_apiv2-2.0.5.tar", last modified: Tue Oct 12 12:21:14 2021, max compression
+gzip compressed data, was "dist/fyers_apiv2-2.0.6.tar", last modified: Fri May  5 06:41:09 2023, max compression
```

## Comparing `fyers_apiv2-2.0.5.tar` & `fyers_apiv2-2.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 piyush    (1000) piyush    (1000)        0 2021-10-12 12:21:14.000000 fyers_apiv2-2.0.5/
--rw-rw-r--   0 piyush    (1000) piyush    (1000)      797 2021-10-12 12:21:14.000000 fyers_apiv2-2.0.5/PKG-INFO
--rwxrwxr-x   0 piyush    (1000) piyush    (1000)      256 2021-08-11 05:22:42.000000 fyers_apiv2-2.0.5/README.md
-drwxrwxr-x   0 piyush    (1000) piyush    (1000)        0 2021-10-12 12:21:14.000000 fyers_apiv2-2.0.5/fyers_api/
-drwxrwxr-x   0 piyush    (1000) piyush    (1000)        0 2021-10-12 12:21:14.000000 fyers_apiv2-2.0.5/fyers_api/Websocket/
--rw-rw-r--   0 piyush    (1000) piyush    (1000)        0 2021-08-11 05:22:42.000000 fyers_apiv2-2.0.5/fyers_api/Websocket/__init__.py
--rw-rw-r--   0 piyush    (1000) piyush    (1000)      988 2021-08-17 12:39:24.000000 fyers_apiv2-2.0.5/fyers_api/Websocket/constants.py
--rw-rw-r--   0 piyush    (1000) piyush    (1000)    11486 2021-10-08 06:44:31.000000 fyers_apiv2-2.0.5/fyers_api/Websocket/ws.py
--rwxrwxr-x   0 piyush    (1000) piyush    (1000)       18 2021-08-11 05:22:42.000000 fyers_apiv2-2.0.5/fyers_api/__init__.py
--rwxrwxr-x   0 piyush    (1000) piyush    (1000)     1563 2021-08-11 05:22:42.000000 fyers_apiv2-2.0.5/fyers_api/accessToken.py
--rwxrwxr-x   0 piyush    (1000) piyush    (1000)      699 2021-08-11 05:22:42.000000 fyers_apiv2-2.0.5/fyers_api/config.py
--rwxrwxr-x   0 piyush    (1000) piyush    (1000)     1010 2021-08-11 05:22:42.000000 fyers_apiv2-2.0.5/fyers_api/fyersFormation.py
--rw-rw-r--   0 piyush    (1000) piyush    (1000)      989 2021-08-11 05:22:42.000000 fyers_apiv2-2.0.5/fyers_api/fyersLog.py
--rwxrwxr-x   0 piyush    (1000) piyush    (1000)    10320 2021-10-06 11:21:37.000000 fyers_apiv2-2.0.5/fyers_api/fyersModel.py
--rwxrwxr-x   0 piyush    (1000) piyush    (1000)     6102 2021-10-06 12:16:42.000000 fyers_apiv2-2.0.5/fyers_api/fyersService.py
--rw-rw-r--   0 piyush    (1000) piyush    (1000)    10517 2021-10-08 06:41:26.000000 fyers_apiv2-2.0.5/fyers_api/tesapi.py
-drwxrwxr-x   0 piyush    (1000) piyush    (1000)        0 2021-10-12 12:21:14.000000 fyers_apiv2-2.0.5/fyers_apiv2.egg-info/
--rw-rw-r--   0 piyush    (1000) piyush    (1000)      797 2021-10-12 12:21:14.000000 fyers_apiv2-2.0.5/fyers_apiv2.egg-info/PKG-INFO
--rw-rw-r--   0 piyush    (1000) piyush    (1000)      470 2021-10-12 12:21:14.000000 fyers_apiv2-2.0.5/fyers_apiv2.egg-info/SOURCES.txt
--rw-rw-r--   0 piyush    (1000) piyush    (1000)        1 2021-10-12 12:21:14.000000 fyers_apiv2-2.0.5/fyers_apiv2.egg-info/dependency_links.txt
--rw-rw-r--   0 piyush    (1000) piyush    (1000)       85 2021-10-12 12:21:14.000000 fyers_apiv2-2.0.5/fyers_apiv2.egg-info/requires.txt
--rw-rw-r--   0 piyush    (1000) piyush    (1000)       10 2021-10-12 12:21:14.000000 fyers_apiv2-2.0.5/fyers_apiv2.egg-info/top_level.txt
--rw-rw-r--   0 piyush    (1000) piyush    (1000)       38 2021-10-12 12:21:14.000000 fyers_apiv2-2.0.5/setup.cfg
--rwxrwxr-x   0 piyush    (1000) piyush    (1000)      838 2021-10-12 11:07:49.000000 fyers_apiv2-2.0.5/setup.py
+drwxrwxr-x   0 ajack     (1000) ajack     (1000)        0 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/
+-rwxrwxr-x   0 ajack     (1000) ajack     (1000)      837 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/setup.py
+-rw-rw-r--   0 ajack     (1000) ajack     (1000)       38 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/setup.cfg
+drwxrwxr-x   0 ajack     (1000) ajack     (1000)        0 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/fyers_api/
+-rwxrwxr-x   0 ajack     (1000) ajack     (1000)     1563 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/fyers_api/accessToken.py
+-rwxrwxr-x   0 ajack     (1000) ajack     (1000)    10320 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/fyers_api/fyersModel.py
+-rwxrwxr-x   0 ajack     (1000) ajack     (1000)       18 2023-05-05 06:39:02.000000 fyers_apiv2-2.0.6/fyers_api/__init__.py
+-rwxrwxr-x   0 ajack     (1000) ajack     (1000)      747 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/fyers_api/config.py
+-rwxrwxr-x   0 ajack     (1000) ajack     (1000)     6338 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/fyers_api/fyersService.py
+drwxrwxr-x   0 ajack     (1000) ajack     (1000)        0 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/fyers_api/Websocket/
+-rw-rw-r--   0 ajack     (1000) ajack     (1000)        0 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/fyers_api/Websocket/__init__.py
+-rw-rw-r--   0 ajack     (1000) ajack     (1000)    11486 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/fyers_api/Websocket/ws.py
+-rw-rw-r--   0 ajack     (1000) ajack     (1000)      988 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/fyers_api/Websocket/constants.py
+-rw-rw-r--   0 ajack     (1000) ajack     (1000)    10517 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/fyers_api/tesapi.py
+-rwxrwxr-x   0 ajack     (1000) ajack     (1000)     1010 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/fyers_api/fyersFormation.py
+-rw-rw-r--   0 ajack     (1000) ajack     (1000)      989 2023-05-05 06:39:27.000000 fyers_apiv2-2.0.6/fyers_api/fyersLog.py
+-rw-rw-r--   0 ajack     (1000) ajack     (1000)      797 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/PKG-INFO
+drwxrwxr-x   0 ajack     (1000) ajack     (1000)        0 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/fyers_apiv2.egg-info/
+-rw-rw-r--   0 ajack     (1000) ajack     (1000)        1 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/fyers_apiv2.egg-info/dependency_links.txt
+-rw-rw-r--   0 ajack     (1000) ajack     (1000)       10 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/fyers_apiv2.egg-info/top_level.txt
+-rw-rw-r--   0 ajack     (1000) ajack     (1000)       85 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/fyers_apiv2.egg-info/requires.txt
+-rw-rw-r--   0 ajack     (1000) ajack     (1000)      470 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/fyers_apiv2.egg-info/SOURCES.txt
+-rw-rw-r--   0 ajack     (1000) ajack     (1000)      797 2023-05-05 06:41:09.000000 fyers_apiv2-2.0.6/fyers_apiv2.egg-info/PKG-INFO
+-rwxrwxr-x   0 ajack     (1000) ajack     (1000)      256 2023-05-05 06:39:02.000000 fyers_apiv2-2.0.6/README.md
```

### Comparing `fyers_apiv2-2.0.5/PKG-INFO` & `fyers_apiv2-2.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers_apiv2
-Version: 2.0.5
+Version: 2.0.6
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 License: UNKNOWN
 Description: README
         ========
```

### Comparing `fyers_apiv2-2.0.5/fyers_api/Websocket/constants.py` & `fyers_apiv2-2.0.6/fyers_api/Websocket/constants.py`

 * *Files identical despite different names*

### Comparing `fyers_apiv2-2.0.5/fyers_api/Websocket/ws.py` & `fyers_apiv2-2.0.6/fyers_api/Websocket/ws.py`

 * *Files identical despite different names*

### Comparing `fyers_apiv2-2.0.5/fyers_api/accessToken.py` & `fyers_apiv2-2.0.6/fyers_api/accessToken.py`

 * *Files identical despite different names*

### Comparing `fyers_apiv2-2.0.5/fyers_api/config.py` & `fyers_apiv2-2.0.6/fyers_api/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 class Config:
     Api = "https://api.fyers.in/api/v2"
-    data_Api= "https://api.fyers.in/data-rest/v2"
-
+    historyDataUrl = "https://api.fyers.in/data-rest/v2"
+    data_Api= "https://api-t1.fyers.in/data"
     get_profile = '/profile'
     tradebook = '/tradebook'
     positions = '/positions'
     holdings = '/holdings'
     convertPosition = '/positions'
     funds = '/funds'
     orders = '/orders'
@@ -16,10 +16,10 @@
     generateAccessToken = '/validate-authcode'
     exitPositions = '/positions'
     generateDataToken = '/data-token'
 
     dataVendorTD = "truedata-ws"
 
     multi_orders = '/orders-multi'
-    history = '/history/'
-    quotes = '/quotes/'
-    market_depth = '/depth/'
+    history = '/history'
+    quotes = '/quotes'
+    market_depth = '/depth'
```

### Comparing `fyers_apiv2-2.0.5/fyers_api/fyersFormation.py` & `fyers_apiv2-2.0.6/fyers_api/fyersFormation.py`

 * *Files identical despite different names*

### Comparing `fyers_apiv2-2.0.5/fyers_api/fyersLog.py` & `fyers_apiv2-2.0.6/fyers_api/fyersLog.py`

 * *Files identical despite different names*

### Comparing `fyers_apiv2-2.0.5/fyers_api/fyersModel.py` & `fyers_apiv2-2.0.6/fyers_api/fyersModel.py`

 * *Files identical despite different names*

### Comparing `fyers_apiv2-2.0.5/fyers_api/fyersService.py` & `fyers_apiv2-2.0.6/fyers_api/fyersService.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,18 @@
         if type(response)==dict:
             return response
         return response.json()
 
     def getCall(self, api, header, data=None,data_flag=False):
         try:
             if data_flag:
-                url = Config.data_Api + api
+                if api == "/history":
+                    url = Config.historyDataUrl + api
+                else:
+                    url = Config.data_Api + api
             else:
                 url = Config.Api + api
             if data is not None:
                 try:
                     url_params = urllib.urlencode(data)
                 except Exception as e:
                     url_params = urllib.parse.urlencode(data)
@@ -89,15 +92,18 @@
             if self.logObj is not None:
                 self.logObj.logEntryFunc(str(int(datetime.now(tz=timezone.utc).timestamp() * 1000)), "getCall", "", "",e)
         return response
 
     def getCall(self, api, header, data=None,data_flag=False):
         try:
             if data_flag:
-                url = Config.data_Api + api
+                if api == '/history':
+                    url = Config.historyDataUrl + api
+                else:
+                    url =  Config.data_Api +api
             else:
                 url = Config.Api + api
             reqClient = httpclient.AsyncHTTPClient()
             if data is not None:
                 try:
                     url_params = urllib.urlencode(data)
                 except Exception as e:
```

### Comparing `fyers_apiv2-2.0.5/fyers_api/tesapi.py` & `fyers_apiv2-2.0.6/fyers_api/tesapi.py`

 * *Files identical despite different names*

### Comparing `fyers_apiv2-2.0.5/fyers_apiv2.egg-info/PKG-INFO` & `fyers_apiv2-2.0.6/fyers_apiv2.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-apiv2
-Version: 2.0.5
+Version: 2.0.6
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 License: UNKNOWN
 Description: README
         ========
```

### Comparing `fyers_apiv2-2.0.5/setup.py` & `fyers_apiv2-2.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='fyers_apiv2',  
-     version='2.0.5',
+     version='2.0.6',
      author="Fyers-Tech",
      author_email="support@fyers.in",
      description="Fyers trading APIs.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/FyersDev/fyers-api-py",
      packages=setuptools.find_packages(),
@@ -21,8 +21,8 @@
                 'websocket-client==1.2.1'
           ],
      classifiers=[
          "Programming Language :: Python :: 3",
          "License :: OSI Approved :: MIT License",
          "Operating System :: OS Independent",
      ],
- )
+ )
```

