# Comparing `tmp/custodes-0.0.2.tar.gz` & `tmp/custodes-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custodes-0.0.2.tar", max compression
+gzip compressed data, was "custodes-0.0.3.tar", max compression
```

## Comparing `custodes-0.0.2.tar` & `custodes-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       17 2023-05-04 13:21:02.450990 custodes-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-05-04 13:19:56.214387 custodes-0.0.2/custodes/__init__.py
--rw-r--r--   0        0        0      893 2023-05-04 23:46:32.000000 custodes-0.0.2/custodes/auth.py
--rw-r--r--   0        0        0     2180 2023-05-05 00:11:48.000000 custodes-0.0.2/custodes/client.py
--rw-r--r--   0        0        0       16 2023-05-04 16:18:32.000000 custodes-0.0.2/custodes/config.py
--rw-r--r--   0        0        0     1864 2023-05-05 02:18:07.951409 custodes-0.0.2/custodes/server.py
--rw-r--r--   0        0        0      356 2023-05-05 02:15:14.782266 custodes-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      713 1970-01-01 00:00:00.000000 custodes-0.0.2/setup.py
--rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 custodes-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       17 2023-05-04 13:21:02.450990 custodes-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 13:19:56.214387 custodes-0.0.3/custodes/__init__.py
+-rw-r--r--   0        0        0      893 2023-05-05 03:02:32.934998 custodes-0.0.3/custodes/auth.py
+-rw-r--r--   0        0        0     2180 2023-05-05 00:11:48.000000 custodes-0.0.3/custodes/client.py
+-rw-r--r--   0        0        0       16 2023-05-04 16:18:32.000000 custodes-0.0.3/custodes/config.py
+-rw-r--r--   0        0        0     1865 2023-05-05 03:25:01.261314 custodes-0.0.3/custodes/server.py
+-rw-r--r--   0        0        0      356 2023-05-05 03:31:00.537871 custodes-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      713 1970-01-01 00:00:00.000000 custodes-0.0.3/setup.py
+-rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 custodes-0.0.3/PKG-INFO
```

### Comparing `custodes-0.0.2/custodes/client.py` & `custodes-0.0.3/custodes/client.py`

 * *Files identical despite different names*

### Comparing `custodes-0.0.2/custodes/server.py` & `custodes-0.0.3/custodes/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 async def _sync_status(message: bytes) -> Dict[str, Any]:
     message_str = message.decode()
     js = cf.js(message_str)
     service_name = js['service_name']
     db = await get_db()
-    await db.set(service_name, js)
+    return db.set(service_name, js)
 
 
 async def generate_summary() -> Dict[str, Any]:
 
     def parse_value(v) -> str:
         def is_okay(time_diff, code: int, seconds: int = 86400) -> bool:
             return time_diff < datetime.timedelta(seconds=seconds) and code == 0
```

### Comparing `custodes-0.0.2/setup.py` & `custodes-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'aiohttp>=3.8.4,<4.0.0',
  'codefast>=23.4.18.13,<24.0.0.0',
  'rich>=13.3.5,<14.0.0',
  'simauth>=0.0.8,<0.0.9']
 
 setup_kwargs = {
     'name': 'custodes',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': '',
     'long_description': '\nApp guardians.\n\n',
     'author': 'tompz',
     'author_email': 'tompz@tompz.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `custodes-0.0.2/PKG-INFO` & `custodes-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custodes
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: tompz
 Author-email: tompz@tompz.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

