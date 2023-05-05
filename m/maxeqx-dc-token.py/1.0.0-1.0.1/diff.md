# Comparing `tmp/maxeqx-dc-token.py-1.0.0.tar.gz` & `tmp/maxeqx-dc-token.py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxeqx-dc-token.py-1.0.0.tar", last modified: Fri May  5 08:37:00 2023, max compression
+gzip compressed data, was "maxeqx-dc-token.py-1.0.1.tar", last modified: Fri May  5 08:59:12 2023, max compression
```

## Comparing `maxeqx-dc-token.py-1.0.0.tar` & `maxeqx-dc-token.py-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 08:37:00.266281 maxeqx-dc-token.py-1.0.0/
--rw-rw-rw-   0        0        0     1051 2023-05-04 14:40:55.000000 maxeqx-dc-token.py-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0       19 2023-05-04 14:44:57.000000 maxeqx-dc-token.py-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      619 2023-05-05 08:37:00.266281 maxeqx-dc-token.py-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-05-05 08:36:36.000000 maxeqx-dc-token.py-1.0.0/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 08:37:00.263282 maxeqx-dc-token.py-1.0.0/maxeqx_dc_token.py.egg-info/
--rw-rw-rw-   0        0        0      619 2023-05-05 08:37:00.000000 maxeqx-dc-token.py-1.0.0/maxeqx_dc_token.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-05-05 08:37:00.000000 maxeqx-dc-token.py-1.0.0/maxeqx_dc_token.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 08:37:00.000000 maxeqx-dc-token.py-1.0.0/maxeqx_dc_token.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-05-05 08:37:00.000000 maxeqx-dc-token.py-1.0.0/maxeqx_dc_token.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 08:37:00.000000 maxeqx-dc-token.py-1.0.0/maxeqx_dc_token.py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 08:37:00.264281 maxeqx-dc-token.py-1.0.0/maxtoken/
--rw-rw-rw-   0        0        0     6010 2023-05-05 08:36:18.000000 maxeqx-dc-token.py-1.0.0/maxtoken/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-05 08:37:00.267281 maxeqx-dc-token.py-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      790 2023-05-05 08:25:01.000000 maxeqx-dc-token.py-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:59:12.571465 maxeqx-dc-token.py-1.0.1/
+-rw-rw-rw-   0        0        0     1051 2023-05-04 14:40:55.000000 maxeqx-dc-token.py-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       19 2023-05-04 14:44:57.000000 maxeqx-dc-token.py-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      619 2023-05-05 08:59:12.569965 maxeqx-dc-token.py-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-05-05 08:36:36.000000 maxeqx-dc-token.py-1.0.1/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 08:59:12.556465 maxeqx-dc-token.py-1.0.1/maxeqx_dc_token.py.egg-info/
+-rw-rw-rw-   0        0        0      619 2023-05-05 08:59:12.000000 maxeqx-dc-token.py-1.0.1/maxeqx_dc_token.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-05-05 08:59:12.000000 maxeqx-dc-token.py-1.0.1/maxeqx_dc_token.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 08:59:12.000000 maxeqx-dc-token.py-1.0.1/maxeqx_dc_token.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-05 08:59:12.000000 maxeqx-dc-token.py-1.0.1/maxeqx_dc_token.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 08:59:12.000000 maxeqx-dc-token.py-1.0.1/maxeqx_dc_token.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 08:59:12.567465 maxeqx-dc-token.py-1.0.1/maxtoken/
+-rw-rw-rw-   0        0        0     5998 2023-05-05 08:58:55.000000 maxeqx-dc-token.py-1.0.1/maxtoken/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-05 08:59:12.571967 maxeqx-dc-token.py-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      783 2023-05-05 08:59:07.000000 maxeqx-dc-token.py-1.0.1/setup.py
```

### Comparing `maxeqx-dc-token.py-1.0.0/LICENSE.txt` & `maxeqx-dc-token.py-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maxeqx-dc-token.py-1.0.0/PKG-INFO` & `maxeqx-dc-token.py-1.0.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxeqx-dc-token.py
-Version: 1.0.0
+Version: 1.0.1
 Summary: This is simple discord token manager.
 Home-page: 
 Author: maxeqx
 Author-email: maxeqxmail@gmail.com
 License: MIT
 Keywords: discord token manager
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `maxeqx-dc-token.py-1.0.0/README.txt` & `maxeqx-dc-token.py-1.0.1/README.txt`

 * *Files identical despite different names*

### Comparing `maxeqx-dc-token.py-1.0.0/maxeqx_dc_token.py.egg-info/PKG-INFO` & `maxeqx-dc-token.py-1.0.1/maxeqx_dc_token.py.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxeqx-dc-token.py
-Version: 1.0.0
+Version: 1.0.1
 Summary: This is simple discord token manager.
 Home-page: 
 Author: maxeqx
 Author-email: maxeqxmail@gmail.com
 License: MIT
 Keywords: discord token manager
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `maxeqx-dc-token.py-1.0.0/maxtoken/__init__.py` & `maxeqx-dc-token.py-1.0.1/maxtoken/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import aiohttp
 import asyncio
 from aioconsole import aprint
-import ssl
 
 class DiscordToken():
     def __init__(self):
         with open('tokens.txt', 'r') as t:
             self.tokens : str = t.read().splitlines()
         with open('proxies.txt', 'r') as p:
             self.proxies : str = p.read().splitlines()
```

### Comparing `maxeqx-dc-token.py-1.0.0/setup.py` & `maxeqx-dc-token.py-1.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,19 +6,19 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='maxeqx-dc-token.py',
-  version='1.0.0',
+  version='1.0.1',
   description='This is simple discord token manager.',
   long_description="Long description and usage is on my github: https://github.com/makseksowny/maxeqx-dc-webhook.",
   url='',  
   author='maxeqx',
   author_email='maxeqxmail@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='discord token manager',
   packages=find_packages(),
-  install_requires=['aiohttp', 'asyncio', 'aioconsole', 'ssl'] 
+  install_requires=['aiohttp', 'asyncio', 'aioconsole'] 
 )
```

