# Comparing `tmp/custodes-0.0.4.tar.gz` & `tmp/custodes-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custodes-0.0.4.tar", max compression
+gzip compressed data, was "custodes-0.0.5.tar", max compression
```

## Comparing `custodes-0.0.4.tar` & `custodes-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       17 2023-05-04 13:21:02.450990 custodes-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-05-04 13:19:56.214387 custodes-0.0.4/custodes/__init__.py
--rw-r--r--   0        0        0      893 2023-05-05 03:02:32.934998 custodes-0.0.4/custodes/auth.py
--rw-r--r--   0        0        0     2249 2023-05-05 03:56:22.965520 custodes-0.0.4/custodes/client.py
--rw-r--r--   0        0        0       16 2023-05-04 16:18:32.000000 custodes-0.0.4/custodes/config.py
--rw-r--r--   0        0        0     1866 2023-05-05 03:54:24.443989 custodes-0.0.4/custodes/server.py
--rw-r--r--   0        0        0      356 2023-05-05 03:58:21.499008 custodes-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      713 1970-01-01 00:00:00.000000 custodes-0.0.4/setup.py
--rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 custodes-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      472 2023-05-05 04:33:11.034987 custodes-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 13:19:56.214387 custodes-0.0.5/custodes/__init__.py
+-rw-r--r--   0        0        0      893 2023-05-05 03:02:32.934998 custodes-0.0.5/custodes/auth.py
+-rw-r--r--   0        0        0     2249 2023-05-05 03:56:22.965520 custodes-0.0.5/custodes/client.py
+-rw-r--r--   0        0        0       16 2023-05-04 16:18:32.000000 custodes-0.0.5/custodes/config.py
+-rw-r--r--   0        0        0     2000 2023-05-05 04:38:59.117136 custodes-0.0.5/custodes/server.py
+-rw-r--r--   0        0        0      376 2023-05-05 04:53:56.740081 custodes-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1211 1970-01-01 00:00:00.000000 custodes-0.0.5/setup.py
+-rw-r--r--   0        0        0     1143 1970-01-01 00:00:00.000000 custodes-0.0.5/PKG-INFO
```

### Comparing `custodes-0.0.4/custodes/auth.py` & `custodes-0.0.5/custodes/auth.py`

 * *Files identical despite different names*

### Comparing `custodes-0.0.4/custodes/client.py` & `custodes-0.0.5/custodes/client.py`

 * *Files identical despite different names*

### Comparing `custodes-0.0.4/custodes/server.py` & `custodes-0.0.5/custodes/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,41 +25,44 @@
     return db.set(service_name, js)
 
 
 async def generate_summary() -> Dict[str, Any]:
 
     def parse_value(v) -> str:
 
-        def is_okay(time_diff, code: int, seconds: int = 86400) -> bool:
-            return time_diff < datetime.timedelta(seconds=seconds) and code == 0
+        def is_okay(time_diff, code: int, expire: int = 86400) -> bool:
+            return time_diff < datetime.timedelta(seconds=expire) and code == 0
 
         js = cf.js(v)
         dtime = js['datetime']
         last_active = datetime.datetime.strptime(dtime, "%Y-%m-%d %H:%M:%S")
         time_diff = datetime.datetime.now() - last_active
         expire = js.get('expire', 86400)
 
         if is_okay(time_diff, js['status']['code'], expire):
             return {
                 'service_name': js['service_name'],
                 'status': 'OK',
                 'last_active': dtime,
                 'ipinfo': js['ipinfo'],
+                'is_okay': True
             }
         else:
             return {
                 'service_name': js['service_name'],
                 'status': 'Error',
                 'last_active': dtime,
                 'ipinfo': js['ipinfo'],
-                'message': js['status']['message']
+                'message': js['status']['message'],
+                'is_okay': False
             }
 
     db = await get_db()
-    return [parse_value(v) for v in db.values()]
+    values = [parse_value(v) for v in db.values()]
+    return sorted(values, key=lambda x: x['is_okay'], reverse=True)
 
 
 async def get():
     return await asyncio.gather(consume(auth.amqp_url, QUEUE, _sync_status),
                                 generate_summary())
```

