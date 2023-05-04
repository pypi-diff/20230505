# Comparing `tmp/twitter-api-client-0.7.8.tar.gz` & `tmp/twitter-api-client-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.7.8.tar", last modified: Wed May  3 18:06:06 2023, max compression
+gzip compressed data, was "twitter-api-client-0.7.9.tar", last modified: Thu May  4 22:30:42 2023, max compression
```

## Comparing `twitter-api-client-0.7.8.tar` & `twitter-api-client-0.7.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-03 18:06:06.413913 twitter-api-client-0.7.8/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-30 17:24:38.000000 twitter-api-client-0.7.8/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     6436 2023-05-03 18:06:06.410580 twitter-api-client-0.7.8/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-05-03 18:06:06.413913 twitter-api-client-0.7.8/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     7678 2023-05-03 18:04:56.000000 twitter-api-client-0.7.8/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-03 18:06:06.410580 twitter-api-client-0.7.8/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-30 17:24:38.000000 twitter-api-client-0.7.8/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    21689 2023-04-30 17:24:38.000000 twitter-api-client-0.7.8/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    27271 2023-04-30 17:24:38.000000 twitter-api-client-0.7.8/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-30 17:24:38.000000 twitter-api-client-0.7.8/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    11024 2023-04-30 17:24:38.000000 twitter-api-client-0.7.8/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     4524 2023-05-03 18:01:10.000000 twitter-api-client-0.7.8/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     3277 2023-04-30 17:24:38.000000 twitter-api-client-0.7.8/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-03 18:06:06.410580 twitter-api-client-0.7.8/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     6436 2023-05-03 18:06:06.000000 twitter-api-client-0.7.8/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-05-03 18:06:06.000000 twitter-api-client-0.7.8/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-05-03 18:06:06.000000 twitter-api-client-0.7.8/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       79 2023-05-03 18:06:06.000000 twitter-api-client-0.7.8/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-05-03 18:06:06.000000 twitter-api-client-0.7.8/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-04 22:30:42.583988 twitter-api-client-0.7.9/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-30 17:24:38.000000 twitter-api-client-0.7.9/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     6951 2023-05-04 22:30:42.583988 twitter-api-client-0.7.9/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-05-04 22:30:42.583988 twitter-api-client-0.7.9/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     8245 2023-05-04 22:26:29.000000 twitter-api-client-0.7.9/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-04 22:30:42.583988 twitter-api-client-0.7.9/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-30 17:24:38.000000 twitter-api-client-0.7.9/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    21689 2023-04-30 17:24:38.000000 twitter-api-client-0.7.9/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    27271 2023-04-30 17:24:38.000000 twitter-api-client-0.7.9/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-30 17:24:38.000000 twitter-api-client-0.7.9/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    11745 2023-05-04 22:19:22.000000 twitter-api-client-0.7.9/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     4524 2023-05-03 18:01:10.000000 twitter-api-client-0.7.9/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     3277 2023-04-30 17:24:38.000000 twitter-api-client-0.7.9/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-04 22:30:42.583988 twitter-api-client-0.7.9/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     6951 2023-05-04 22:30:42.000000 twitter-api-client-0.7.9/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-05-04 22:30:42.000000 twitter-api-client-0.7.9/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-05-04 22:30:42.000000 twitter-api-client-0.7.9/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       79 2023-05-04 22:30:42.000000 twitter-api-client-0.7.9/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-05-04 22:30:42.000000 twitter-api-client-0.7.9/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.7.8/LICENSE` & `twitter-api-client-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.8/PKG-INFO` & `twitter-api-client-0.7.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.7.8
+Version: 0.7.9
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -196,14 +196,29 @@
     444444,
 ])
 
 
 
 # trends
 scraper.trends()
+
+
+from twitter.scraper import Scraper
+from twitter.constants import Operation
+
+email, username, password = ...,...,...
+scraper = Scraper(email, username, password, debug=1, save=True)
+
+operation = Operation.Followers
+user_id = 44196397
+cursor = '1765001818576065118|1654241854176100129' # example cursor
+limit = 250  # arbitrary limit for demonstration
+
+follower_subset, last_cursor = scraper.resume_pagination(scraper.session, user_id, operation, limit=limit, cursor=cursor)
+# use last_cursor to resume pagination
 ```
 
 #### Search
 
 ```python   
 from twitter.search import Search
```

### Comparing `twitter-api-client-0.7.8/setup.py` & `twitter-api-client-0.7.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.7.8",
+    version="0.7.9",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     Implementation of Twitter's v1, v2, and GraphQL APIs
     
     Includes tools to **scrape**, **automate**, and **search**.
 
@@ -202,14 +202,29 @@
         444444,
     ])
     
 
     
     # trends
     scraper.trends()
+
+
+    from twitter.scraper import Scraper
+    from twitter.constants import Operation
+    
+    email, username, password = ...,...,...
+    scraper = Scraper(email, username, password, debug=1, save=True)
+    
+    operation = Operation.Followers
+    user_id = 44196397
+    cursor = '1765001818576065118|1654241854176100129' # example cursor
+    limit = 250  # arbitrary limit for demonstration
+    
+    follower_subset, last_cursor = scraper.resume_pagination(scraper.session, user_id, operation, limit=limit, cursor=cursor)
+    # use last_cursor to resume pagination
     ```
     
     #### Search
     
     ```python   
     from twitter.search import Search
```

### Comparing `twitter-api-client-0.7.8/twitter/account.py` & `twitter-api-client-0.7.9/twitter/account.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.8/twitter/constants.py` & `twitter-api-client-0.7.9/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.8/twitter/login.py` & `twitter-api-client-0.7.9/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.8/twitter/scraper.py` & `twitter-api-client-0.7.9/twitter/scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 import logging.config
 import math
 import platform
 import time
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from pathlib import Path
+from typing import List
 from urllib.parse import urlsplit
 
 import httpx
 import orjson
 from httpx import AsyncClient, Response
 from tqdm import tqdm
 
@@ -136,45 +137,63 @@
     def _run(self, ids: list[int | str], operation: tuple, limit=None):
         return asyncio.run(self._process(ids, operation, limit))
 
     async def _process(self, ids: list[int | str], op: tuple, limit: int | None) -> list:
         async with AsyncClient(headers=get_headers(self.session)) as s:
             return await asyncio.gather(*(self._paginate(s, _id, op, limit) for _id in ids))
 
-    async def _paginate(self, session: AsyncClient, _id: int | str | list[int], operation: tuple,
-                        limit: int | None) -> list[dict]:
+    async def _paginate(self, session: AsyncClient, _id: int | str, operation: tuple,
+                        limit: int | None, **kwargs) -> list[dict] | tuple[list[dict], str]:
 
-        r = await self._query(session, _id, operation)
-        initial_data = r.json()
-        res = [initial_data]
-        ids = set(find_key(initial_data, 'rest_id'))
+        cursor = kwargs.get('cursor')
+        is_resuming = False
         dups = 0
         DUP_LIMIT = 3
 
-        cursor = get_cursor(initial_data)
+        if cursor:
+            is_resuming = True
+            res = []
+            ids = set()
+        else:
+            r = await self._query(session, _id, operation)
+            initial_data = r.json()
+            res = [initial_data]
+            ids = set(find_key(initial_data, 'rest_id'))
+            cursor = get_cursor(initial_data)
+
         while (dups < DUP_LIMIT) and cursor:
             prev_len = len(ids)
             if prev_len >= limit:
-                return res
+                # return res
+                break
 
             r = await self._query(session, _id, operation, cursor=cursor)
             data = r.json()
 
             cursor = get_cursor(data)
             ids |= set(find_key(data, 'rest_id'))
 
             if self.debug:
                 logger.debug(f'cursor: {cursor}\tunique results: {len(ids)}')
 
             if prev_len == len(ids):
                 dups += 1
 
             res.append(data)
+
+        if is_resuming:
+            return res, cursor
         return res
 
+    def resume_pagination(self, *args, **kwargs):
+        async def _resume(session: AsyncClient, _id: int | str, operation: tuple, limit=math.inf, **kwargs) -> tuple:
+            session = AsyncClient(headers=get_headers(session), cookies=self.session.cookies)
+            return await self._paginate(session, _id, operation, limit, **kwargs)
+        return asyncio.run(_resume(*args, **kwargs))
+
     async def _query(self, session: AsyncClient, _id: int | str | list, operation: tuple, **kwargs) -> Response:
         qid, op, k = operation
         params = {k: orjson.dumps(v).decode() for k, v in {
             'variables': {k: _id} | Operation.default_variables | kwargs,
             'features': Operation.default_features,
         }.items()}
         r = await session.get(f'{self.api}/{qid}/{op}', params=params)
```

### Comparing `twitter-api-client-0.7.8/twitter/search.py` & `twitter-api-client-0.7.9/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.8/twitter/util.py` & `twitter-api-client-0.7.9/twitter/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.8/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.7.9/twitter_api_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.7.8
+Version: 0.7.9
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -196,14 +196,29 @@
     444444,
 ])
 
 
 
 # trends
 scraper.trends()
+
+
+from twitter.scraper import Scraper
+from twitter.constants import Operation
+
+email, username, password = ...,...,...
+scraper = Scraper(email, username, password, debug=1, save=True)
+
+operation = Operation.Followers
+user_id = 44196397
+cursor = '1765001818576065118|1654241854176100129' # example cursor
+limit = 250  # arbitrary limit for demonstration
+
+follower_subset, last_cursor = scraper.resume_pagination(scraper.session, user_id, operation, limit=limit, cursor=cursor)
+# use last_cursor to resume pagination
 ```
 
 #### Search
 
 ```python   
 from twitter.search import Search
```

