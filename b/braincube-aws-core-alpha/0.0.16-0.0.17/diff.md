# Comparing `tmp/braincube-aws-core-alpha-0.0.16.tar.gz` & `tmp/braincube-aws-core-alpha-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braincube-aws-core-alpha-0.0.16.tar", last modified: Thu May  4 09:15:52 2023, max compression
+gzip compressed data, was "braincube-aws-core-alpha-0.0.17.tar", last modified: Fri May  5 16:04:48 2023, max compression
```

## Comparing `braincube-aws-core-alpha-0.0.16.tar` & `braincube-aws-core-alpha-0.0.17.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:15:52.526057 braincube-aws-core-alpha-0.0.16/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 13:41:49.000000 braincube-aws-core-alpha-0.0.16/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9298 2023-05-04 09:15:52.526335 braincube-aws-core-alpha-0.0.16/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8348 2023-05-03 19:09:10.000000 braincube-aws-core-alpha-0.0.16/README.md
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-02 13:42:37.000000 braincube-aws-core-alpha-0.0.16/pyproject.toml
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1086 2023-05-04 09:15:52.527896 braincube-aws-core-alpha-0.0.16/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 13:44:20.000000 braincube-aws-core-alpha-0.0.16/setup.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:15:52.507211 braincube-aws-core-alpha-0.0.16/src/
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:15:52.512078 braincube-aws-core-alpha-0.0.16/src/braincube_aws_core_alpha.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9298 2023-05-04 09:15:52.000000 braincube-aws-core-alpha-0.0.16/src/braincube_aws_core_alpha.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-04 09:15:52.000000 braincube-aws-core-alpha-0.0.16/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-04 09:15:52.000000 braincube-aws-core-alpha-0.0.16/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-04 09:15:52.000000 braincube-aws-core-alpha-0.0.16/src/braincube_aws_core_alpha.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-04 09:15:52.000000 braincube-aws-core-alpha-0.0.16/src/braincube_aws_core_alpha.egg-info/top_level.txt
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:15:52.512663 braincube-aws-core-alpha-0.0.16/src/core/
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.16/src/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:15:52.515682 braincube-aws-core-alpha-0.0.16/src/core/dal/
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.16/src/core/dal/__init__.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     1289 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.16/src/core/dal/data.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)      281 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.16/src/core/dal/database_errors.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     2257 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.16/src/core/dal/postgres_connection.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)    26358 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.16/src/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:15:52.518090 braincube-aws-core-alpha-0.0.16/src/core/di/
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.16/src/core/di/__init__.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)      623 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.16/src/core/di/data.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     3796 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.16/src/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:15:52.522021 braincube-aws-core-alpha-0.0.16/src/core/rest/
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.16/src/core/rest/__init__.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     2883 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.16/src/core/rest/app_controller.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     3741 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.16/src/core/rest/app_module.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.16/src/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:15:52.525255 braincube-aws-core-alpha-0.0.16/src/core/utils/
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.16/src/core/utils/__init__.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)      580 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.16/src/core/utils/convert.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     1437 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.16/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-05 16:04:48.164987 braincube-aws-core-alpha-0.0.17/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 13:41:49.000000 braincube-aws-core-alpha-0.0.17/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9298 2023-05-05 16:04:48.165167 braincube-aws-core-alpha-0.0.17/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8348 2023-05-03 19:09:10.000000 braincube-aws-core-alpha-0.0.17/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-02 13:42:37.000000 braincube-aws-core-alpha-0.0.17/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1086 2023-05-05 16:04:48.167142 braincube-aws-core-alpha-0.0.17/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 13:44:20.000000 braincube-aws-core-alpha-0.0.17/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-05 16:04:48.148603 braincube-aws-core-alpha-0.0.17/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-05 16:04:48.152801 braincube-aws-core-alpha-0.0.17/src/braincube_aws_core_alpha.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9298 2023-05-05 16:04:48.000000 braincube-aws-core-alpha-0.0.17/src/braincube_aws_core_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-05 16:04:48.000000 braincube-aws-core-alpha-0.0.17/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-05 16:04:48.000000 braincube-aws-core-alpha-0.0.17/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-05 16:04:48.000000 braincube-aws-core-alpha-0.0.17/src/braincube_aws_core_alpha.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-05 16:04:48.000000 braincube-aws-core-alpha-0.0.17/src/braincube_aws_core_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-05 16:04:48.153156 braincube-aws-core-alpha-0.0.17/src/core/
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.17/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-05 16:04:48.155622 braincube-aws-core-alpha-0.0.17/src/core/dal/
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.17/src/core/dal/__init__.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     1289 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.17/src/core/dal/data.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)      281 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.17/src/core/dal/database_errors.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     2257 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.17/src/core/dal/postgres_connection.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)    26674 2023-05-05 15:30:20.000000 braincube-aws-core-alpha-0.0.17/src/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-05 16:04:48.158036 braincube-aws-core-alpha-0.0.17/src/core/di/
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.17/src/core/di/__init__.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)      623 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.17/src/core/di/data.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     3796 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.17/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-05 16:04:48.162364 braincube-aws-core-alpha-0.0.17/src/core/rest/
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.17/src/core/rest/__init__.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     2883 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.17/src/core/rest/app_controller.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     3741 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.17/src/core/rest/app_module.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.17/src/core/rest/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-05 16:04:48.164299 braincube-aws-core-alpha-0.0.17/src/core/utils/
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.17/src/core/utils/__init__.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)      580 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.17/src/core/utils/convert.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     1437 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.17/src/core/utils/data.py
```

### Comparing `braincube-aws-core-alpha-0.0.16/LICENSE` & `braincube-aws-core-alpha-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.16/PKG-INFO` & `braincube-aws-core-alpha-0.0.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.16
+Version: 0.0.17
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-alpha-0.0.16/README.md` & `braincube-aws-core-alpha-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.16/setup.cfg` & `braincube-aws-core-alpha-0.0.17/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = braincube-aws-core-alpha
-version = 0.0.16
+version = 0.0.17
 author = Braincube
 author_email = v.boudis@braincube.gr
 description = Microframework for python aws lambdas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/braincube-common/core-aws.git
 license = MIT
```

### Comparing `braincube-aws-core-alpha-0.0.16/src/braincube_aws_core_alpha.egg-info/PKG-INFO` & `braincube-aws-core-alpha-0.0.17/src/braincube_aws_core_alpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.16
+Version: 0.0.17
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-alpha-0.0.16/src/braincube_aws_core_alpha.egg-info/SOURCES.txt` & `braincube-aws-core-alpha-0.0.17/src/braincube_aws_core_alpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.16/src/core/dal/data.py` & `braincube-aws-core-alpha-0.0.17/src/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.16/src/core/dal/postgres_connection.py` & `braincube-aws-core-alpha-0.0.17/src/core/dal/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.16/src/core/dal/postgres_repository.py` & `braincube-aws-core-alpha-0.0.17/src/core/dal/postgres_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import time
 import math
 import itertools
 from typing import Optional, List, Dict, Union, Tuple
 
-from pypika import PostgreSQLQuery, Table, Field, Criterion, EmptyCriterion, CustomFunction, functions as fn
+from pydantic import BaseModel
 from pypika.queries import QueryBuilder
+from pypika import PostgreSQLQuery, Table, Field, Criterion, EmptyCriterion, CustomFunction, functions as fn
 
 from ..utils.data import Order, OrderType, Condition, ConditionType, Page, Pageable, Paging, Top, Metadata
 from .data import Key, Schema, Relation, SaveType, Column, StatementField
 from .database_errors import DatabaseError, DeleteError, SaveError
 from .postgres_connection import Pool, Connection
 
 
@@ -323,25 +324,27 @@
             page_no = total_pages
             records = await self._fetch(q.limit(page.page_size).offset((page_no - 1) * page.page_size),
                                         connection=connection)
 
         return Page(records, Paging(page_no, page.page_size, total_pages, count),
                     Metadata(int((time.time() - start) * 1000)))
 
-    async def _update(self, data: Dict[str, any],
+    async def _update(self, data: Union[Dict[str, any], BaseModel],
                       criterion: Criterion,
                       returning_aliases: Optional[List[str]] = None,
                       connection: Optional[Connection] = None) -> Optional[List[Dict[str, any]]]:
 
         if isinstance(criterion, EmptyCriterion):
             raise SaveError("update without conditions is not allowed")
 
         uq = PostgreSQLQuery.update(self._master_table[1])
 
-        for v, k in self._filter_save_data(data, SaveType.update).items():
+        data_ = data.dict(by_alias=True, exclude_unset=True) if data is BaseModel else data.copy()
+
+        for v, k in self._filter_save_data(data_, SaveType.update).items():
             uq = uq.set(v, k)
         uq = uq.where(criterion)
 
         return await self._execute(uq, returning_aliases, connection)
 
     async def _delete(self, criterion: Criterion,
                       returning_aliases: Optional[List[str]] = None,
@@ -452,26 +455,29 @@
         criterion = self._conditions_to_criterion(conditions)
 
         if connection:
             return await self._find_all_page(connection, aliases, criterion, page, order)
         async with self._pool.acquire() as connection_:
             return await self._find_all_page(connection_, aliases, criterion, page, order)
 
-    async def insert(self, data: Dict[str, any],
+    async def insert(self, data: Union[Dict[str, any], BaseModel],
                      returning_aliases: Optional[List[str]] = None,
                      connection: Optional[Connection] = None) -> Dict[str, any]:
         """Insert one record from dictionary.
         :param data: Master column aliases with values.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to insert-constraints or no master column is specified.
         :return: Execution results as dictionary.
         """
 
-        data_ = self._filter_save_data(data, SaveType.insert)
+        data_ = self._filter_save_data(
+            data.dict(by_alias=True, exclude_unset=True) if data is BaseModel else data.copy(),
+            SaveType.insert
+        )
 
         iq = PostgreSQLQuery \
             .into(self._master_table[1]) \
             .columns(list(data_.keys())) \
             .insert(list(data_.values()))
 
         records = await self._execute(iq, returning_aliases, connection)
@@ -512,15 +518,15 @@
             .columns(list(column_names.keys()))
 
         for d in data:
             iq = iq.insert([d[i] for i in column_names.values()])
 
         return await self._execute(iq, returning_aliases, connection)
 
-    async def update(self, data: Dict[str, any],
+    async def update(self, data: Union[Dict[str, any], BaseModel],
                      conditions: List[Condition],
                      returning_aliases: Optional[List[str]] = None,
                      connection: Optional[Connection] = None) -> Optional[List[Dict[str, any]]]:
         """Update records with new data according conditions.
         :param data: Master column aliases with values.
         :param conditions: List of filters that will be applied into the query.
         :param returning_aliases: Query returning data.
@@ -530,15 +536,15 @@
         """
 
         criterion = self._conditions_to_criterion(conditions, select=False)
 
         return await self._update(data, criterion, returning_aliases, connection)
 
     async def update_by_id(self, key: Key,
-                           data: Dict[str, any],
+                           data: Union[Dict[str, any], BaseModel],
                            returning_aliases: Optional[List[str]] = None,
                            connection: Optional[Connection] = None) -> Optional[Dict[str, any]]:
         """Update records with new data according to passed key.
         :param key: Record identifier.
         :param data: Master column aliases with values.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
```

### Comparing `braincube-aws-core-alpha-0.0.16/src/core/di/data.py` & `braincube-aws-core-alpha-0.0.17/src/core/di/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.16/src/core/di/injector.py` & `braincube-aws-core-alpha-0.0.17/src/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.16/src/core/rest/app_controller.py` & `braincube-aws-core-alpha-0.0.17/src/core/rest/app_controller.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.16/src/core/rest/app_module.py` & `braincube-aws-core-alpha-0.0.17/src/core/rest/app_module.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.16/src/core/rest/data.py` & `braincube-aws-core-alpha-0.0.17/src/core/rest/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.16/src/core/utils/convert.py` & `braincube-aws-core-alpha-0.0.17/src/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.16/src/core/utils/data.py` & `braincube-aws-core-alpha-0.0.17/src/core/utils/data.py`

 * *Files identical despite different names*

