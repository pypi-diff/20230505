# Comparing `tmp/custodes-0.0.1.tar.gz` & `tmp/custodes-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custodes-0.0.1.tar", max compression
+gzip compressed data, was "custodes-0.0.2.tar", max compression
```

## Comparing `custodes-0.0.1.tar` & `custodes-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       17 2023-05-04 13:21:02.000000 custodes-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-04 13:19:56.000000 custodes-0.0.1/custodes/__init__.py
--rw-r--r--   0        0        0      893 2023-05-04 23:46:32.313984 custodes-0.0.1/custodes/auth.py
--rw-r--r--   0        0        0     2180 2023-05-05 00:11:48.813711 custodes-0.0.1/custodes/client.py
--rw-r--r--   0        0        0       16 2023-05-04 16:18:32.541207 custodes-0.0.1/custodes/config.py
--rw-r--r--   0        0        0     1788 2023-05-05 00:13:13.200003 custodes-0.0.1/custodes/server.py
--rw-r--r--   0        0        0      355 2023-05-04 16:17:04.004037 custodes-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      706 2023-05-05 00:14:56.048128 custodes-0.0.1/setup.py
--rw-r--r--   0        0        0      601 2023-05-05 00:14:56.048418 custodes-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       17 2023-05-04 13:21:02.450990 custodes-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 13:19:56.214387 custodes-0.0.2/custodes/__init__.py
+-rw-r--r--   0        0        0      893 2023-05-04 23:46:32.000000 custodes-0.0.2/custodes/auth.py
+-rw-r--r--   0        0        0     2180 2023-05-05 00:11:48.000000 custodes-0.0.2/custodes/client.py
+-rw-r--r--   0        0        0       16 2023-05-04 16:18:32.000000 custodes-0.0.2/custodes/config.py
+-rw-r--r--   0        0        0     1864 2023-05-05 02:18:07.951409 custodes-0.0.2/custodes/server.py
+-rw-r--r--   0        0        0      356 2023-05-05 02:15:14.782266 custodes-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      713 1970-01-01 00:00:00.000000 custodes-0.0.2/setup.py
+-rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 custodes-0.0.2/PKG-INFO
```

### Comparing `custodes-0.0.1/custodes/auth.py` & `custodes-0.0.2/custodes/auth.py`

 * *Files identical despite different names*

### Comparing `custodes-0.0.1/custodes/client.py` & `custodes-0.0.2/custodes/client.py`

 * *Files identical despite different names*

### Comparing `custodes-0.0.1/custodes/server.py` & `custodes-0.0.2/custodes/server.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,33 +24,34 @@
     db = await get_db()
     await db.set(service_name, js)
 
 
 async def generate_summary() -> Dict[str, Any]:
 
     def parse_value(v) -> str:
+        def is_okay(time_diff, code: int, seconds: int = 86400) -> bool:
+            return time_diff < datetime.timedelta(seconds=seconds) and code == 0
+
         js = cf.js(v)
         dtime = js['datetime']
         last_active = datetime.datetime.strptime(dtime, "%Y-%m-%d %H:%M:%S")
         time_diff = datetime.datetime.now() - last_active
+        expire = js.get('expire', 86400)
 
-        def is_okay(time_diff, code: int) -> bool:
-            return time_diff > datetime.timedelta(minutes=10) and code == 0
-
-        if is_okay(time_diff, js['status']['code']):
+        if is_okay(time_diff, js['status']['code'], expire):
             return {
                 'service_name': js['service_name'],
-                'status': 'ok',
+                'status': 'OK',
                 'last_active': dtime,
                 'ipinfo': js['ipinfo'],
             }
         else:
             return {
                 'service_name': js['service_name'],
-                'status': 'error',
+                'status': 'Error',
                 'last_active': dtime,
                 'ipinfo': js['ipinfo'],
                 'message': js['status']['message']
             }
 
     db = await get_db()
     return [parse_value(v) for v in db.values()]
```

### Comparing `custodes-0.0.1/setup.py` & `custodes-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,22 +12,22 @@
  'aiohttp>=3.8.4,<4.0.0',
  'codefast>=23.4.18.13,<24.0.0.0',
  'rich>=13.3.5,<14.0.0',
  'simauth>=0.0.8,<0.0.9']
 
 setup_kwargs = {
     'name': 'custodes',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': '',
     'long_description': '\nApp guardians.\n\n',
     'author': 'tompz',
-    'author_email': '....@tompz.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'author_email': 'tompz@tompz.com',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `custodes-0.0.1/PKG-INFO` & `custodes-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: custodes
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: tompz
-Author-email: ....@tompz.com
+Author-email: tompz@tompz.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aio-pika (>=9.0.5,<10.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: codefast (>=23.4.18.13,<24.0.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: simauth (>=0.0.8,<0.0.9)
 Description-Content-Type: text/markdown
```

