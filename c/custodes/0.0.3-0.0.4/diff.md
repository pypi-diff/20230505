# Comparing `tmp/custodes-0.0.3.tar.gz` & `tmp/custodes-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custodes-0.0.3.tar", max compression
+gzip compressed data, was "custodes-0.0.4.tar", max compression
```

## Comparing `custodes-0.0.3.tar` & `custodes-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       17 2023-05-04 13:21:02.450990 custodes-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-05-04 13:19:56.214387 custodes-0.0.3/custodes/__init__.py
--rw-r--r--   0        0        0      893 2023-05-05 03:02:32.934998 custodes-0.0.3/custodes/auth.py
--rw-r--r--   0        0        0     2180 2023-05-05 00:11:48.000000 custodes-0.0.3/custodes/client.py
--rw-r--r--   0        0        0       16 2023-05-04 16:18:32.000000 custodes-0.0.3/custodes/config.py
--rw-r--r--   0        0        0     1865 2023-05-05 03:25:01.261314 custodes-0.0.3/custodes/server.py
--rw-r--r--   0        0        0      356 2023-05-05 03:31:00.537871 custodes-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      713 1970-01-01 00:00:00.000000 custodes-0.0.3/setup.py
--rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 custodes-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       17 2023-05-04 13:21:02.450990 custodes-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 13:19:56.214387 custodes-0.0.4/custodes/__init__.py
+-rw-r--r--   0        0        0      893 2023-05-05 03:02:32.934998 custodes-0.0.4/custodes/auth.py
+-rw-r--r--   0        0        0     2249 2023-05-05 03:56:22.965520 custodes-0.0.4/custodes/client.py
+-rw-r--r--   0        0        0       16 2023-05-04 16:18:32.000000 custodes-0.0.4/custodes/config.py
+-rw-r--r--   0        0        0     1866 2023-05-05 03:54:24.443989 custodes-0.0.4/custodes/server.py
+-rw-r--r--   0        0        0      356 2023-05-05 03:58:21.499008 custodes-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      713 1970-01-01 00:00:00.000000 custodes-0.0.4/setup.py
+-rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 custodes-0.0.4/PKG-INFO
```

### Comparing `custodes-0.0.3/custodes/auth.py` & `custodes-0.0.4/custodes/auth.py`

 * *Files identical despite different names*

### Comparing `custodes-0.0.3/custodes/client.py` & `custodes-0.0.4/custodes/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,37 +29,39 @@
                     f'https://ipinfo.io/json?token={auth.ipinfo_token}'
             ) as resp:
                 js = await resp.json()
                 cf.js.write(js, fp)
                 return await _parse_ip(js)
 
 
-async def _post_status(service_name: str, status: Dict[str,
-                                                       Any]) -> Dict[str, Any]:
+async def _post_status(service_name: str, status: Dict[str, Any],
+                       expire: int) -> Dict[str, Any]:
     assert isinstance(status, dict)
     assert 'code' in status
     assert 'message' in status
 
     datetime = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
     js = {
         'service_name': service_name,
         'status': status,
+        'expire': expire,
         'datetime': datetime,
         'ipinfo': await ipinfo()
     }
     return await publish(auth.amqp_url, QUEUE, str(js))
 
 
 async def post(service_name: str,
                status: Dict[str, Any],
+               expire: int = 86400,
                loop: bool = False,
                sleep_period=60) -> None:
     while True:
         try:
-            js = await _post_status(service_name, status)
+            js = await _post_status(service_name, status, expire)
             cf.info(js)
             if not loop:
                 return js
         except Exception as e:
             import traceback
             cf.error({
                 'error': 'post status failed',
@@ -69,10 +71,10 @@
 
         await asyncio.sleep(sleep_period)
 
 
 if __name__ == '__main__':
 
     async def main():
-        print(await post('test', {'code': 0, 'message': 'test'}, True, 0.1))
+        print(await post('test', {'code': 0, 'message': 'test'}, loop=True, sleep_period=0.1))
 
     asyncio.run(main())
```

### Comparing `custodes-0.0.3/custodes/server.py` & `custodes-0.0.4/custodes/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     db = await get_db()
     return db.set(service_name, js)
 
 
 async def generate_summary() -> Dict[str, Any]:
 
     def parse_value(v) -> str:
+
         def is_okay(time_diff, code: int, seconds: int = 86400) -> bool:
             return time_diff < datetime.timedelta(seconds=seconds) and code == 0
 
         js = cf.js(v)
         dtime = js['datetime']
         last_active = datetime.datetime.strptime(dtime, "%Y-%m-%d %H:%M:%S")
         time_diff = datetime.datetime.now() - last_active
```

### Comparing `custodes-0.0.3/setup.py` & `custodes-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'aiohttp>=3.8.4,<4.0.0',
  'codefast>=23.4.18.13,<24.0.0.0',
  'rich>=13.3.5,<14.0.0',
  'simauth>=0.0.8,<0.0.9']
 
 setup_kwargs = {
     'name': 'custodes',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': '',
     'long_description': '\nApp guardians.\n\n',
     'author': 'tompz',
     'author_email': 'tompz@tompz.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `custodes-0.0.3/PKG-INFO` & `custodes-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custodes
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Author: tompz
 Author-email: tompz@tompz.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

