# Comparing `tmp/custodes-0.0.5.tar.gz` & `tmp/custodes-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custodes-0.0.5.tar", max compression
+gzip compressed data, was "custodes-0.0.6.tar", max compression
```

## Comparing `custodes-0.0.5.tar` & `custodes-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      472 2023-05-05 04:33:11.034987 custodes-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-05-04 13:19:56.214387 custodes-0.0.5/custodes/__init__.py
--rw-r--r--   0        0        0      893 2023-05-05 03:02:32.934998 custodes-0.0.5/custodes/auth.py
--rw-r--r--   0        0        0     2249 2023-05-05 03:56:22.965520 custodes-0.0.5/custodes/client.py
--rw-r--r--   0        0        0       16 2023-05-04 16:18:32.000000 custodes-0.0.5/custodes/config.py
--rw-r--r--   0        0        0     2000 2023-05-05 04:38:59.117136 custodes-0.0.5/custodes/server.py
--rw-r--r--   0        0        0      376 2023-05-05 04:53:56.740081 custodes-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1211 1970-01-01 00:00:00.000000 custodes-0.0.5/setup.py
--rw-r--r--   0        0        0     1143 1970-01-01 00:00:00.000000 custodes-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      472 2023-05-05 04:33:11.034987 custodes-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 13:19:56.214387 custodes-0.0.6/custodes/__init__.py
+-rw-r--r--   0        0        0      893 2023-05-05 03:02:32.934998 custodes-0.0.6/custodes/auth.py
+-rw-r--r--   0        0        0     2249 2023-05-05 03:56:22.965520 custodes-0.0.6/custodes/client.py
+-rw-r--r--   0        0        0       16 2023-05-04 16:18:32.000000 custodes-0.0.6/custodes/config.py
+-rw-r--r--   0        0        0     2000 2023-05-05 04:38:59.117136 custodes-0.0.6/custodes/server.py
+-rw-r--r--   0        0        0      375 2023-05-05 10:08:43.377045 custodes-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 custodes-0.0.6/setup.py
+-rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 custodes-0.0.6/PKG-INFO
```

### Comparing `custodes-0.0.5/custodes/auth.py` & `custodes-0.0.6/custodes/auth.py`

 * *Files identical despite different names*

### Comparing `custodes-0.0.5/custodes/client.py` & `custodes-0.0.6/custodes/client.py`

 * *Files identical despite different names*

### Comparing `custodes-0.0.5/custodes/server.py` & `custodes-0.0.6/custodes/server.py`

 * *Files identical despite different names*

### Comparing `custodes-0.0.5/setup.py` & `custodes-0.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 {'': ['*']}
 
 install_requires = \
 ['aio-pika>=9.0.5,<10.0.0',
  'aiohttp>=3.8.4,<4.0.0',
  'codefast>=23.4.18.13,<24.0.0.0',
  'rich>=13.3.5,<14.0.0',
- 'simauth>=0.0.8,<0.0.9',
+ 'simauth==0.0.9',
  'urllib3==1.26.15']
 
 setup_kwargs = {
     'name': 'custodes',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': '',
     'long_description': "\nApp guardians.\n\n# Usage\n```python\nimport asyncio\nfrom typing import Any, Dict\n\nfrom codefast.asyncio.rabbitmq import consume\nfrom rich import print\n\nfrom custodes.server import get\nfrom custodes.client import post\n\nasync def main():\n    return await asyncio.gather(\n        post('custodes server', {'code': 0, 'message': 'OK'}, loop=True, expire=120),\n        get()\n    )\n\nif __name__ == '__main__':\n    cf.info('custodes server started...')\n    asyncio.run(main())\n\n```\n",
     'author': 'tompz',
     'author_email': 'tompz@tompz.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `custodes-0.0.5/PKG-INFO` & `custodes-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: custodes
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Author: tompz
 Author-email: tompz@tompz.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aio-pika (>=9.0.5,<10.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: codefast (>=23.4.18.13,<24.0.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
-Requires-Dist: simauth (>=0.0.8,<0.0.9)
+Requires-Dist: simauth (==0.0.9)
 Requires-Dist: urllib3 (==1.26.15)
 Description-Content-Type: text/markdown
 
 
 App guardians.
 
 # Usage
```

