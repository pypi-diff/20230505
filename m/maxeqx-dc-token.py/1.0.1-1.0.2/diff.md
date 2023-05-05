# Comparing `tmp/maxeqx-dc-token.py-1.0.1.tar.gz` & `tmp/maxeqx-dc-token.py-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxeqx-dc-token.py-1.0.1.tar", last modified: Fri May  5 08:59:12 2023, max compression
+gzip compressed data, was "maxeqx-dc-token.py-1.0.2.tar", last modified: Fri May  5 09:13:51 2023, max compression
```

## Comparing `maxeqx-dc-token.py-1.0.1.tar` & `maxeqx-dc-token.py-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 08:59:12.571465 maxeqx-dc-token.py-1.0.1/
--rw-rw-rw-   0        0        0     1051 2023-05-04 14:40:55.000000 maxeqx-dc-token.py-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       19 2023-05-04 14:44:57.000000 maxeqx-dc-token.py-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      619 2023-05-05 08:59:12.569965 maxeqx-dc-token.py-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-05-05 08:36:36.000000 maxeqx-dc-token.py-1.0.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 08:59:12.556465 maxeqx-dc-token.py-1.0.1/maxeqx_dc_token.py.egg-info/
--rw-rw-rw-   0        0        0      619 2023-05-05 08:59:12.000000 maxeqx-dc-token.py-1.0.1/maxeqx_dc_token.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-05-05 08:59:12.000000 maxeqx-dc-token.py-1.0.1/maxeqx_dc_token.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 08:59:12.000000 maxeqx-dc-token.py-1.0.1/maxeqx_dc_token.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-05 08:59:12.000000 maxeqx-dc-token.py-1.0.1/maxeqx_dc_token.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 08:59:12.000000 maxeqx-dc-token.py-1.0.1/maxeqx_dc_token.py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 08:59:12.567465 maxeqx-dc-token.py-1.0.1/maxtoken/
--rw-rw-rw-   0        0        0     5998 2023-05-05 08:58:55.000000 maxeqx-dc-token.py-1.0.1/maxtoken/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-05 08:59:12.571967 maxeqx-dc-token.py-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      783 2023-05-05 08:59:07.000000 maxeqx-dc-token.py-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:13:51.553842 maxeqx-dc-token.py-1.0.2/
+-rw-rw-rw-   0        0        0     1051 2023-05-04 14:40:55.000000 maxeqx-dc-token.py-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       19 2023-05-04 14:44:57.000000 maxeqx-dc-token.py-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      619 2023-05-05 09:13:51.550341 maxeqx-dc-token.py-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-05-05 08:36:36.000000 maxeqx-dc-token.py-1.0.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 09:13:51.545836 maxeqx-dc-token.py-1.0.2/maxeqx_dc_token.py.egg-info/
+-rw-rw-rw-   0        0        0      619 2023-05-05 09:13:51.000000 maxeqx-dc-token.py-1.0.2/maxeqx_dc_token.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-05-05 09:13:51.000000 maxeqx-dc-token.py-1.0.2/maxeqx_dc_token.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 09:13:51.000000 maxeqx-dc-token.py-1.0.2/maxeqx_dc_token.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-05-05 09:13:51.000000 maxeqx-dc-token.py-1.0.2/maxeqx_dc_token.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 09:13:51.000000 maxeqx-dc-token.py-1.0.2/maxeqx_dc_token.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 09:13:51.547835 maxeqx-dc-token.py-1.0.2/maxtoken/
+-rw-rw-rw-   0        0        0     5858 2023-05-05 09:13:02.000000 maxeqx-dc-token.py-1.0.2/maxtoken/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-05 09:13:51.554836 maxeqx-dc-token.py-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      793 2023-05-05 09:13:49.000000 maxeqx-dc-token.py-1.0.2/setup.py
```

### Comparing `maxeqx-dc-token.py-1.0.1/LICENSE.txt` & `maxeqx-dc-token.py-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maxeqx-dc-token.py-1.0.1/PKG-INFO` & `maxeqx-dc-token.py-1.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxeqx-dc-token.py
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is simple discord token manager.
 Home-page: 
 Author: maxeqx
 Author-email: maxeqxmail@gmail.com
 License: MIT
 Keywords: discord token manager
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `maxeqx-dc-token.py-1.0.1/README.txt` & `maxeqx-dc-token.py-1.0.2/README.txt`

 * *Files identical despite different names*

### Comparing `maxeqx-dc-token.py-1.0.1/maxeqx_dc_token.py.egg-info/PKG-INFO` & `maxeqx-dc-token.py-1.0.2/maxeqx_dc_token.py.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxeqx-dc-token.py
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is simple discord token manager.
 Home-page: 
 Author: maxeqx
 Author-email: maxeqxmail@gmail.com
 License: MIT
 Keywords: discord token manager
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `maxeqx-dc-token.py-1.0.1/maxtoken/__init__.py` & `maxeqx-dc-token.py-1.0.2/maxtoken/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,18 +69,17 @@
                     'Sec-Fetch-Mode': 'cors',
                     'Sec-Fetch-Site': 'same-origin',
                     'TE': 'trailers',
                 }
                 async with aiohttp.ClientSession() as session:
                     async with session.post(f"https://canary.discord.com/api/v9/invites/{code}", headers=headers, json={}) as resp:
                         if resp.status == 200:
-                            await aprint("Joined successfully")
+                            return
                         elif resp.status == 429:
                             j = await resp.json()
-                            await aprint(f"Ratelimited for {j['retry_after']} seconds")
                             await asyncio.sleep(j['retry_after'])
                         elif resp.status == 403:
-                            await aprint("Locked token")
+                            return
                         else:
                             j = await resp.json()
                             await aprint(resp.status, j,)
                     await asyncio.sleep(0.7)
```

### Comparing `maxeqx-dc-token.py-1.0.1/setup.py` & `maxeqx-dc-token.py-1.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,19 +6,19 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='maxeqx-dc-token.py',
-  version='1.0.1',
+  version='1.0.2',
   description='This is simple discord token manager.',
   long_description="Long description and usage is on my github: https://github.com/makseksowny/maxeqx-dc-webhook.",
   url='',  
   author='maxeqx',
   author_email='maxeqxmail@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='discord token manager',
   packages=find_packages(),
-  install_requires=['aiohttp', 'asyncio', 'aioconsole'] 
+  install_requires=['aiohttp', 'asyncio', 'aioconsole', 'Brotli'] 
 )
```

