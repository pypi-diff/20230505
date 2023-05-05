# Comparing `tmp/maxeqx-dc-webhook.py-1.0.8.tar.gz` & `tmp/maxeqx-dc-webhook.py-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxeqx-dc-webhook.py-1.0.8.tar", last modified: Thu May  4 20:12:39 2023, max compression
+gzip compressed data, was "maxeqx-dc-webhook.py-1.0.9.tar", last modified: Fri May  5 07:55:21 2023, max compression
```

## Comparing `maxeqx-dc-webhook.py-1.0.8.tar` & `maxeqx-dc-webhook.py-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 20:12:39.273499 maxeqx-dc-webhook.py-1.0.8/
--rw-rw-rw-   0        0        0     1051 2023-05-04 14:40:55.000000 maxeqx-dc-webhook.py-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0       19 2023-05-04 14:44:57.000000 maxeqx-dc-webhook.py-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      626 2023-05-04 20:12:39.268501 maxeqx-dc-webhook.py-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      607 2023-05-04 18:20:45.000000 maxeqx-dc-webhook.py-1.0.8/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 20:12:39.263999 maxeqx-dc-webhook.py-1.0.8/maxeqx_dc_webhook.py.egg-info/
--rw-rw-rw-   0        0        0      626 2023-05-04 20:12:39.000000 maxeqx-dc-webhook.py-1.0.8/maxeqx_dc_webhook.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-05-04 20:12:39.000000 maxeqx-dc-webhook.py-1.0.8/maxeqx_dc_webhook.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 20:12:39.000000 maxeqx-dc-webhook.py-1.0.8/maxeqx_dc_webhook.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-04 20:12:39.000000 maxeqx-dc-webhook.py-1.0.8/maxeqx_dc_webhook.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-04 20:12:39.000000 maxeqx-dc-webhook.py-1.0.8/maxeqx_dc_webhook.py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 20:12:39.265499 maxeqx-dc-webhook.py-1.0.8/maxwebhook/
--rw-rw-rw-   0        0        0     1732 2023-05-04 20:10:21.000000 maxeqx-dc-webhook.py-1.0.8/maxwebhook/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-04 20:12:39.273999 maxeqx-dc-webhook.py-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      766 2023-05-04 19:59:09.000000 maxeqx-dc-webhook.py-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:55:21.755629 maxeqx-dc-webhook.py-1.0.9/
+-rw-rw-rw-   0        0        0     1051 2023-05-04 14:40:55.000000 maxeqx-dc-webhook.py-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       19 2023-05-04 14:44:57.000000 maxeqx-dc-webhook.py-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      626 2023-05-05 07:55:21.753630 maxeqx-dc-webhook.py-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      733 2023-05-05 07:54:23.000000 maxeqx-dc-webhook.py-1.0.9/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 07:55:21.738628 maxeqx-dc-webhook.py-1.0.9/maxeqx_dc_webhook.py.egg-info/
+-rw-rw-rw-   0        0        0      626 2023-05-05 07:55:21.000000 maxeqx-dc-webhook.py-1.0.9/maxeqx_dc_webhook.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-05-05 07:55:21.000000 maxeqx-dc-webhook.py-1.0.9/maxeqx_dc_webhook.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 07:55:21.000000 maxeqx-dc-webhook.py-1.0.9/maxeqx_dc_webhook.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 07:55:21.000000 maxeqx-dc-webhook.py-1.0.9/maxeqx_dc_webhook.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-05 07:55:21.000000 maxeqx-dc-webhook.py-1.0.9/maxeqx_dc_webhook.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 07:55:21.750639 maxeqx-dc-webhook.py-1.0.9/maxwebhook/
+-rw-rw-rw-   0        0        0      789 2023-05-05 07:55:10.000000 maxeqx-dc-webhook.py-1.0.9/maxwebhook/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-05 07:55:21.756628 maxeqx-dc-webhook.py-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      766 2023-05-05 07:53:15.000000 maxeqx-dc-webhook.py-1.0.9/setup.py
```

### Comparing `maxeqx-dc-webhook.py-1.0.8/LICENSE.txt` & `maxeqx-dc-webhook.py-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maxeqx-dc-webhook.py-1.0.8/PKG-INFO` & `maxeqx-dc-webhook.py-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxeqx-dc-webhook.py
-Version: 1.0.8
+Version: 1.0.9
 Summary: This is simple webhook sender in discord.
 Home-page: 
 Author: maxeqx
 Author-email: maxeqxmail@gmail.com
 License: MIT
 Keywords: discord webhook sender
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `maxeqx-dc-webhook.py-1.0.8/README.txt` & `maxeqx-dc-webhook.py-1.0.9/README.txt`

 * *Files 17% similar despite different names*

```diff
@@ -30,9 +30,15 @@
 
 #setting avatar url
 webhook.avatar_url = 'avatarurl'
 
 #setting message
 webhook.message = 'message'
 
+#setting embed title
+webhook.embedtitle = 'title'
+
+#setting embed description
+webhook.embeddescription = 'description'
+
 #sending message
 await webhook.send()
```

### Comparing `maxeqx-dc-webhook.py-1.0.8/maxeqx_dc_webhook.py.egg-info/PKG-INFO` & `maxeqx-dc-webhook.py-1.0.9/maxeqx_dc_webhook.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxeqx-dc-webhook.py
-Version: 1.0.8
+Version: 1.0.9
 Summary: This is simple webhook sender in discord.
 Home-page: 
 Author: maxeqx
 Author-email: maxeqxmail@gmail.com
 License: MIT
 Keywords: discord webhook sender
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `maxeqx-dc-webhook.py-1.0.8/maxwebhook/__init__.py` & `maxeqx-dc-webhook.py-1.0.9/maxwebhook/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,42 +10,19 @@
         self.embeddescription : str = None
     def send(self):     
         url = self.url
 
         headers = {
         "Content-Type": "application/json"
         }
-
-        if self.embeddescription or self.embedtitle != None:
-            embed = {
-            "description": self.embeddescription,
-            "title": self.embedtitle
-            }
-            data = {
-            "username" : self.username,
-            "avatar_url" : self.avatar_url,
-            "embeds": [embed]
-            }
-            result = requests.post(url, json=data, headers=headers)
-            result.raise_for_status()
-        elif self.embeddescription and self.embedtitle and self.message != None:
-            embed = {
-            "description": self.embeddescription,
-            "title": self.embedtitle,
-            "content": self.message
-            }
-            data = {
-            "username" : self.username,
-            "avatar_url" : self.avatar_url,
-            "embeds": [embed]
-            }
-            result = requests.post(url, json=data, headers=headers)
-            result.raise_for_status()
-        else:
-            if self.message != None:
-                data = {
-                    "username" : self.username,
-                    "avatar_url" : self.avatar_url,
-                    "content" : self.message
-                }
-                result = requests.post(url, json=data, headers=headers)
-                result.raise_for_status
+        embed = {
+        "description": self.embeddescription,
+        "title": self.embedtitle,
+        "content": self.message
+        }
+        data = {
+        "username" : self.username,
+        "avatar_url" : self.avatar_url,
+        "embeds": [embed]
+        }
+        result = requests.post(url, json=data, headers=headers)
+        result.raise_for_status()
```

### Comparing `maxeqx-dc-webhook.py-1.0.8/setup.py` & `maxeqx-dc-webhook.py-1.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='maxeqx-dc-webhook.py',
-  version='1.0.8',
+  version='1.0.9',
   description='This is simple webhook sender in discord.',
   long_description="Long description and usage is on my github: https://github.com/makseksowny/maxeqx-dc-webhook.",
   url='',  
   author='maxeqx',
   author_email='maxeqxmail@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

