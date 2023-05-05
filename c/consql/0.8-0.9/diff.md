# Comparing `tmp/consql-0.8.tar.gz` & `tmp/consql-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/consql-0.8.tar", last modified: Mon May  2 08:25:04 2022, max compression
+gzip compressed data, was "dist/consql-0.9.tar", last modified: Sun Jun 26 20:27:42 2022, max compression
```

## Comparing `consql-0.8.tar` & `consql-0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kosyachniy   (502) staff       (20)        0 2022-05-02 08:25:04.000000 consql-0.8/
--rw-r--r--   0 kosyachniy   (502) staff       (20)     1020 2022-05-02 08:25:04.000000 consql-0.8/PKG-INFO
--rw-r--r--   0 kosyachniy   (502) staff       (20)      195 2022-04-23 20:32:27.000000 consql-0.8/README.md
-drwxr-xr-x   0 kosyachniy   (502) staff       (20)        0 2022-05-02 08:25:04.000000 consql-0.8/consql/
--rw-r--r--   0 kosyachniy   (502) staff       (20)      246 2022-05-02 08:24:54.000000 consql-0.8/consql/__init__.py
--rw-r--r--   0 kosyachniy   (502) staff       (20)    14618 2022-04-30 20:10:15.000000 consql-0.8/consql/_db.py
--rw-r--r--   0 kosyachniy   (502) staff       (20)     1435 2022-04-27 10:13:49.000000 consql-0.8/consql/_json.py
--rw-r--r--   0 kosyachniy   (502) staff       (20)     9041 2022-04-30 22:34:51.000000 consql-0.8/consql/_sql.py
--rw-r--r--   0 kosyachniy   (502) staff       (20)     2588 2022-04-27 22:03:53.000000 consql-0.8/consql/coerces.py
--rw-r--r--   0 kosyachniy   (502) staff       (20)     1338 2022-04-30 19:53:06.000000 consql-0.8/consql/errors.py
--rw-r--r--   0 kosyachniy   (502) staff       (20)      493 2022-04-27 10:29:48.000000 consql-0.8/consql/main.py
--rw-r--r--   0 kosyachniy   (502) staff       (20)    21342 2022-05-02 08:24:21.000000 consql-0.8/consql/model.py
--rw-r--r--   0 kosyachniy   (502) staff       (20)     1530 2022-04-23 20:58:44.000000 consql-0.8/consql/table.py
--rw-r--r--   0 kosyachniy   (502) staff       (20)     1325 2022-04-28 14:34:20.000000 consql-0.8/consql/types.py
-drwxr-xr-x   0 kosyachniy   (502) staff       (20)        0 2022-05-02 08:25:04.000000 consql-0.8/consql.egg-info/
--rw-r--r--   0 kosyachniy   (502) staff       (20)     1020 2022-05-02 08:25:04.000000 consql-0.8/consql.egg-info/PKG-INFO
--rw-r--r--   0 kosyachniy   (502) staff       (20)      329 2022-05-02 08:25:04.000000 consql-0.8/consql.egg-info/SOURCES.txt
--rw-r--r--   0 kosyachniy   (502) staff       (20)        1 2022-05-02 08:25:04.000000 consql-0.8/consql.egg-info/dependency_links.txt
--rw-r--r--   0 kosyachniy   (502) staff       (20)       73 2022-05-02 08:25:04.000000 consql-0.8/consql.egg-info/requires.txt
--rw-r--r--   0 kosyachniy   (502) staff       (20)        7 2022-05-02 08:25:04.000000 consql-0.8/consql.egg-info/top_level.txt
--rw-r--r--   0 kosyachniy   (502) staff       (20)       38 2022-05-02 08:25:04.000000 consql-0.8/setup.cfg
--rw-r--r--   0 kosyachniy   (502) staff       (20)     1702 2022-04-28 17:54:47.000000 consql-0.8/setup.py
+drwxr-xr-x   0 kosyachniy   (502) staff       (20)        0 2022-06-26 20:27:42.000000 consql-0.9/
+-rw-r--r--   0 kosyachniy   (502) staff       (20)     1166 2022-06-26 20:27:42.000000 consql-0.9/PKG-INFO
+-rw-r--r--   0 kosyachniy   (502) staff       (20)      293 2022-06-26 18:10:45.000000 consql-0.9/README.md
+drwxr-xr-x   0 kosyachniy   (502) staff       (20)        0 2022-06-26 20:27:42.000000 consql-0.9/consql/
+-rw-r--r--   0 kosyachniy   (502) staff       (20)      246 2022-06-26 20:27:28.000000 consql-0.9/consql/__init__.py
+-rw-r--r--   0 kosyachniy   (502) staff       (20)    14618 2022-04-30 20:10:15.000000 consql-0.9/consql/_db.py
+-rw-r--r--   0 kosyachniy   (502) staff       (20)     1435 2022-04-27 10:13:49.000000 consql-0.9/consql/_json.py
+-rw-r--r--   0 kosyachniy   (502) staff       (20)     9142 2022-06-26 20:15:35.000000 consql-0.9/consql/_sql.py
+-rw-r--r--   0 kosyachniy   (502) staff       (20)     2588 2022-04-27 22:03:53.000000 consql-0.9/consql/coerces.py
+-rw-r--r--   0 kosyachniy   (502) staff       (20)     1338 2022-04-30 19:53:06.000000 consql-0.9/consql/errors.py
+-rw-r--r--   0 kosyachniy   (502) staff       (20)      493 2022-04-27 10:29:48.000000 consql-0.9/consql/main.py
+-rw-r--r--   0 kosyachniy   (502) staff       (20)    22272 2022-06-26 20:26:29.000000 consql-0.9/consql/model.py
+-rw-r--r--   0 kosyachniy   (502) staff       (20)     1530 2022-04-23 20:58:44.000000 consql-0.9/consql/table.py
+-rw-r--r--   0 kosyachniy   (502) staff       (20)     1325 2022-04-28 14:34:20.000000 consql-0.9/consql/types.py
+drwxr-xr-x   0 kosyachniy   (502) staff       (20)        0 2022-06-26 20:27:42.000000 consql-0.9/consql.egg-info/
+-rw-r--r--   0 kosyachniy   (502) staff       (20)     1166 2022-06-26 20:27:42.000000 consql-0.9/consql.egg-info/PKG-INFO
+-rw-r--r--   0 kosyachniy   (502) staff       (20)      329 2022-06-26 20:27:42.000000 consql-0.9/consql.egg-info/SOURCES.txt
+-rw-r--r--   0 kosyachniy   (502) staff       (20)        1 2022-06-26 20:27:42.000000 consql-0.9/consql.egg-info/dependency_links.txt
+-rw-r--r--   0 kosyachniy   (502) staff       (20)       73 2022-06-26 20:27:42.000000 consql-0.9/consql.egg-info/requires.txt
+-rw-r--r--   0 kosyachniy   (502) staff       (20)        7 2022-06-26 20:27:42.000000 consql-0.9/consql.egg-info/top_level.txt
+-rw-r--r--   0 kosyachniy   (502) staff       (20)       38 2022-06-26 20:27:42.000000 consql-0.9/setup.cfg
+-rw-r--r--   0 kosyachniy   (502) staff       (20)     1702 2022-04-28 17:54:47.000000 consql-0.9/setup.py
```

### Comparing `consql-0.8/PKG-INFO` & `consql-0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: consql
-Version: 0.8
+Version: 0.9
 Summary: PostgreSQL Async ORM for Python
 Home-page: https://github.com/kosyachniy/consql
 Author: Alexey Poloz
 Author-email: polozhev@mail.ru
 License: MIT
 Project-URL: Source, https://github.com/kosyachniy/consql
 Description: # ConSQL
         PostgreSQL Async ORM for Python
         
         [GitHub](https://github.com/kosyachniy/consql)
          | [PyPI](https://pypi.org/project/consql/)
         
         [View ORM for MongoDB →](https://pypi.org/project/consys/)
         
+        ## First connect & create DB
+        ```
+        psql -h localhost -p 5432 -U postgres
+        CREATE DATABASE main;
+        ```
+        
 Keywords: async,orm,python,postgresql,sql,types,checking,oop
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `consql-0.8/consql/_db.py` & `consql-0.9/consql/_db.py`

 * *Files identical despite different names*

### Comparing `consql-0.8/consql/_json.py` & `consql-0.9/consql/_json.py`

 * *Files identical despite different names*

### Comparing `consql-0.8/consql/_sql.py` & `consql-0.9/consql/_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,15 @@
 
         self._env = jinja2.Environment(
             loader=loader,
             extensions=[
                 _BindSQLFragmentExtension
             ],
         )
+        self._env.filters['datetime'] = lambda i: datetime.datetime.strptime(i, '%Y-%m-%d %H:%M:%S')
 
         if json_encoder:
             self.json_encoder = json_encoder
         else:
             self.json_encoder = json.dumps
 
         self._cache = {}
```

### Comparing `consql-0.8/consql/coerces.py` & `consql-0.9/consql/coerces.py`

 * *Files identical despite different names*

### Comparing `consql-0.8/consql/errors.py` & `consql-0.9/consql/errors.py`

 * *Files identical despite different names*

### Comparing `consql-0.8/consql/model.py` & `consql-0.9/consql/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -563,17 +563,41 @@
     def _force_limit(limit):
         if limit is None:
             return CURSOR_LIMIT
         if limit > CURSOR_LIMIT:
             return CURSOR_LIMIT
         if limit < 1:
             return 1
-
         return limit
 
+class CursorExt(Cursor):
+    serial = Attribute(types=str, coerce=str)
+    direction = Attribute(types=str, required=True, default='DESC')
+
+    def __init__(self, row = None, **kw):
+        if row is None:
+            row = {}
+        if isinstance(row, CursorExt):
+            row = row.pure_python()
+
+        if isinstance(row, str):
+            data = unpack(TOKEN, row)
+
+            if data is None:
+                row = {}
+            elif isinstance(data, dict):
+                row = data.get('cursor', {})
+            else:
+                row = {}
+
+        row = copy.copy(row)
+        row['limit'] = self._force_limit(row.get('limit', None))
+
+        super().__init__(row, **kw)
+
 
 class BaseModel(Base):
     """ Base model """
 
     @property
     @abstractmethod
     def database(self):
@@ -716,49 +740,53 @@
             'sqlbase': cls.sqlbase(),
             'shard': db.get('shard'),
         }
         if 'sort' in kw and isinstance(kw['sort'], str):
             kw['sort'] = [kw['sort']]
 
         if ids:
-            tmp = 'load.sqlt'
+            tmp = 'get.sqlt'
             kw = {
                 **kw,
                 'key_def': (by,) if isinstance(by, str) else by,
                 'key': ids,
                 'key_tuple': ids if isinstance(ids, (list, tuple)) else [ids],
                 'class': cls,
             }
 
-        elif offset is not None:
-            tmp = 'list.sqlt'
+        elif offset is not None or by == 'pager':
+            tmp = 'pager.sqlt'
             pager = Pager(offset=offset, limit=limit, **kw)
             kw['pager'] = pager
 
+        elif cursor is not None or by == 'cursor':
+            tmp = 'cursor.sqlt'
+            cursor = CursorExt(cursor or kw)
+            kw['cursor'] = cursor
+
         else:
             tmp = 'full.sqlt'
-            cursor = Cursor(kw)
-            kw['cursor'] = cursor
+            cursor = CursorExt(kw)
 
         sql, args = sqlt(tmp, kw)
 
         async with dbh(**db) as conn:
             data = await conn.fetch(sql, *args)
 
-        if ids:
+        if tmp == 'get.sqlt':
             if not data:
                 return None
 
             data = cls(data[0])
             if isinstance(db, dict) and 'shard' in db:
                 data.actual_shard = db['shard']
 
             return data
 
-        if offset is not None:
+        if tmp == 'pager.sqlt':
             if not pager.disabled:
                 if len(data) <= pager.limit:
                     pager.latest = True
                 while len(data) > pager.limit:
                     pager.latest = False
                     data.pop(len(data) - 1)
 
@@ -766,14 +794,16 @@
                 data[i] = cls(row)
 
             pager.list = data
 
             return pager.list
 
         cursor.list = [cls(x) for x in data]
+        if cursor.list:
+            cursor.serial = str(cursor.list[-1].id)
 
         if isinstance(db, dict) and 'shard' in db:
             for item in cursor.list:
                 item.actual_shard = db['shard']
 
         return cursor.list, cursor.cursor_str
```

### Comparing `consql-0.8/consql/table.py` & `consql-0.9/consql/table.py`

 * *Files identical despite different names*

### Comparing `consql-0.8/consql/types.py` & `consql-0.9/consql/types.py`

 * *Files identical despite different names*

### Comparing `consql-0.8/consql.egg-info/PKG-INFO` & `consql-0.9/consql.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: consql
-Version: 0.8
+Version: 0.9
 Summary: PostgreSQL Async ORM for Python
 Home-page: https://github.com/kosyachniy/consql
 Author: Alexey Poloz
 Author-email: polozhev@mail.ru
 License: MIT
 Project-URL: Source, https://github.com/kosyachniy/consql
 Description: # ConSQL
         PostgreSQL Async ORM for Python
         
         [GitHub](https://github.com/kosyachniy/consql)
          | [PyPI](https://pypi.org/project/consql/)
         
         [View ORM for MongoDB →](https://pypi.org/project/consys/)
         
+        ## First connect & create DB
+        ```
+        psql -h localhost -p 5432 -U postgres
+        CREATE DATABASE main;
+        ```
+        
 Keywords: async,orm,python,postgresql,sql,types,checking,oop
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `consql-0.8/setup.py` & `consql-0.9/setup.py`

 * *Files identical despite different names*

