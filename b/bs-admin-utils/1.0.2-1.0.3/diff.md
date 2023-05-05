# Comparing `tmp/bs_admin_utils-1.0.2.tar.gz` & `tmp/bs_admin_utils-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_admin_utils-1.0.2.tar", last modified: Tue Apr 11 08:24:44 2023, max compression
+gzip compressed data, was "bs_admin_utils-1.0.3.tar", last modified: Fri May  5 05:03:54 2023, max compression
```

## Comparing `bs_admin_utils-1.0.2.tar` & `bs_admin_utils-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-04-11 08:24:44.862003 bs_admin_utils-1.0.2/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     1067 2023-04-07 03:25:03.000000 bs_admin_utils-1.0.2/LICENSE
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       35 2023-04-07 04:04:08.000000 bs_admin_utils-1.0.2/MANIFEST.in
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      260 2023-04-11 08:24:44.862003 bs_admin_utils-1.0.2/PKG-INFO
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      206 2023-04-07 03:35:29.000000 bs_admin_utils-1.0.2/README.md
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-04-11 08:24:44.862003 bs_admin_utils-1.0.2/bs_admin_utils/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       13 2023-04-07 03:39:05.000000 bs_admin_utils-1.0.2/bs_admin_utils/__init__.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     3966 2023-04-11 08:24:04.000000 bs_admin_utils-1.0.2/bs_admin_utils/api.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      490 2023-04-07 04:11:32.000000 bs_admin_utils-1.0.2/bs_admin_utils/decorators.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     1034 2023-04-07 03:48:50.000000 bs_admin_utils-1.0.2/bs_admin_utils/model.py
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-04-11 08:24:44.862003 bs_admin_utils-1.0.2/bs_admin_utils/static/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)   367112 2023-04-07 03:52:07.000000 bs_admin_utils-1.0.2/bs_admin_utils/static/arial.ttf
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     2320 2023-04-07 04:36:50.000000 bs_admin_utils-1.0.2/bs_admin_utils/vercode.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     2868 2023-04-07 04:10:45.000000 bs_admin_utils-1.0.2/bs_admin_utils/websocket.py
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-04-11 08:24:44.862003 bs_admin_utils-1.0.2/bs_admin_utils.egg-info/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      260 2023-04-11 08:24:44.000000 bs_admin_utils-1.0.2/bs_admin_utils.egg-info/PKG-INFO
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      448 2023-04-11 08:24:44.000000 bs_admin_utils-1.0.2/bs_admin_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-04-11 08:24:44.000000 bs_admin_utils-1.0.2/bs_admin_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       44 2023-04-11 08:24:44.000000 bs_admin_utils-1.0.2/bs_admin_utils.egg-info/requires.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       15 2023-04-11 08:24:44.000000 bs_admin_utils-1.0.2/bs_admin_utils.egg-info/top_level.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-04-11 08:24:44.000000 bs_admin_utils-1.0.2/bs_admin_utils.egg-info/zip-safe
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       38 2023-04-11 08:24:44.862003 bs_admin_utils-1.0.2/setup.cfg
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      620 2023-04-11 08:24:34.000000 bs_admin_utils-1.0.2/setup.py
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-05-05 05:03:54.856180 bs_admin_utils-1.0.3/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     1067 2023-04-07 03:25:03.000000 bs_admin_utils-1.0.3/LICENSE
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       35 2023-04-07 04:04:08.000000 bs_admin_utils-1.0.3/MANIFEST.in
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      260 2023-05-05 05:03:54.856180 bs_admin_utils-1.0.3/PKG-INFO
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      206 2023-04-07 03:35:29.000000 bs_admin_utils-1.0.3/README.md
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-05-05 05:03:54.852180 bs_admin_utils-1.0.3/bs_admin_utils/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       13 2023-04-07 03:39:05.000000 bs_admin_utils-1.0.3/bs_admin_utils/__init__.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     4046 2023-05-05 05:01:20.000000 bs_admin_utils-1.0.3/bs_admin_utils/api.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      490 2023-04-07 04:11:32.000000 bs_admin_utils-1.0.3/bs_admin_utils/decorators.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     1034 2023-04-07 03:48:50.000000 bs_admin_utils-1.0.3/bs_admin_utils/model.py
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-05-05 05:03:54.856180 bs_admin_utils-1.0.3/bs_admin_utils/static/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)   367112 2023-04-07 03:52:07.000000 bs_admin_utils-1.0.3/bs_admin_utils/static/arial.ttf
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     2320 2023-04-07 04:36:50.000000 bs_admin_utils-1.0.3/bs_admin_utils/vercode.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     2868 2023-04-07 04:10:45.000000 bs_admin_utils-1.0.3/bs_admin_utils/websocket.py
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-05-05 05:03:54.856180 bs_admin_utils-1.0.3/bs_admin_utils.egg-info/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      260 2023-05-05 05:03:54.000000 bs_admin_utils-1.0.3/bs_admin_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      448 2023-05-05 05:03:54.000000 bs_admin_utils-1.0.3/bs_admin_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-05-05 05:03:54.000000 bs_admin_utils-1.0.3/bs_admin_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       44 2023-05-05 05:03:54.000000 bs_admin_utils-1.0.3/bs_admin_utils.egg-info/requires.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       15 2023-05-05 05:03:54.000000 bs_admin_utils-1.0.3/bs_admin_utils.egg-info/top_level.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-05-05 05:03:54.000000 bs_admin_utils-1.0.3/bs_admin_utils.egg-info/zip-safe
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       38 2023-05-05 05:03:54.856180 bs_admin_utils-1.0.3/setup.cfg
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      620 2023-05-05 05:03:18.000000 bs_admin_utils-1.0.3/setup.py
```

### Comparing `bs_admin_utils-1.0.2/LICENSE` & `bs_admin_utils-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.0.2/bs_admin_utils/api.py` & `bs_admin_utils-1.0.3/bs_admin_utils/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from asyncio import get_running_loop
+from asyncio import create_task, get_running_loop, wait
 from beanie.odm.queries.find import FindMany
 from blacksheep import file, Request
 from blacksheep.server.controllers import APIController, delete, get, patch, post, put, ws
 from blacksheep.server.responses import not_found
 from kikiutils.aiofile import aread_file
 from kikiutils.check import isbytes, isfile
 from kikiutils.file import get_file_mime, save_file_as_bytesio
@@ -41,20 +41,22 @@
         )
 
         await self.process_data(data, model)
         data['id'] = str(model.id)
         return dict_key_snake_to_camel(data)
 
     async def models_to_data(self, count: int, models: FindMany[ModelType]):
+        tasks = [create_task(self.model_to_dict(model)) async for model in models]
+
+        if tasks:
+            await wait(tasks)
+
         return {
             'count': count,
-            'data': [
-                await self.model_to_dict(model)
-                async for model in models
-            ]
+            'data': [task.result() for task in tasks]
         }
 
     async def process_data(self, data: dict[str], model: ModelType):
         pass
 
     # Apis
```

### Comparing `bs_admin_utils-1.0.2/bs_admin_utils/model.py` & `bs_admin_utils-1.0.3/bs_admin_utils/model.py`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.0.2/bs_admin_utils/static/arial.ttf` & `bs_admin_utils-1.0.3/bs_admin_utils/static/arial.ttf`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.0.2/bs_admin_utils/vercode.py` & `bs_admin_utils-1.0.3/bs_admin_utils/vercode.py`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.0.2/bs_admin_utils/websocket.py` & `bs_admin_utils-1.0.3/bs_admin_utils/websocket.py`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.0.2/setup.py` & `bs_admin_utils-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ],
     packages=find_packages(),
     package_data={
         'bs_admin_utils': ['*.ttf']
     },
     include_package_data=True,
     zip_safe=True,
-    version='1.0.2',
+    version='1.0.3',
     description='Blacksheep admin backend utils classes and function.',
     author='kiki-kanri',
     author_email='a470666@gmail.com',
     keywords=[],
     install_requires=[
         'beanie',
         'blacksheep',
```

