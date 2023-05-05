# Comparing `tmp/HawaData-0.3.4.tar.gz` & `tmp/HawaData-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.3.4.tar", last modified: Fri May  5 07:43:51 2023, max compression
+gzip compressed data, was "HawaData-0.3.6.tar", last modified: Fri May  5 08:29:15 2023, max compression
```

## Comparing `HawaData-0.3.4.tar` & `HawaData-0.3.6.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.138455 HawaData-0.3.4/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.125710 HawaData-0.3.4/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2140 2023-05-05 07:43:51.000000 HawaData-0.3.4/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      765 2023-05-05 07:43:51.000000 HawaData-0.3.4/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-05 07:43:51.000000 HawaData-0.3.4/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)      141 2023-05-05 07:43:51.000000 HawaData-0.3.4/HawaData.egg-info/requires.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)       10 2023-05-05 07:43:51.000000 HawaData-0.3.4/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     2140 2023-05-05 07:43:51.138052 HawaData-0.3.4/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.3.4/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.126475 HawaData-0.3.4/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.3.4/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.128938 HawaData-0.3.4/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.3.4/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2842 2022-12-11 02:48:15.000000 HawaData-0.3.4/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.3.4/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.3.4/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.130755 HawaData-0.3.4/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.3.4/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     8828 2023-05-05 07:06:02.000000 HawaData-0.3.4/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5032 2023-04-25 09:59:36.000000 HawaData-0.3.4/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2738 2023-05-05 07:06:32.000000 HawaData-0.3.4/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.3.4/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.131959 HawaData-0.3.4/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.3.4/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.3.4/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.3.4/hawa/data/school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.133183 HawaData-0.3.4/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.3.4/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    23013 2023-05-05 07:06:02.000000 HawaData-0.3.4/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.3.4/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-05 07:43:51.138584 HawaData-0.3.4/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      875 2022-12-02 07:10:09.000000 HawaData-0.3.4/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.134795 HawaData-0.3.4/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2022-12-01 08:54:31.000000 HawaData-0.3.4/test/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      654 2022-12-02 04:24:16.000000 HawaData-0.3.4/test/mock.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.135466 HawaData-0.3.4/test/test_common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:19.000000 HawaData-0.3.4/test/test_common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      770 2023-04-13 03:56:08.000000 HawaData-0.3.4/test/test_common/test_common_data.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.136250 HawaData-0.3.4/test/test_data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:40.000000 HawaData-0.3.4/test/test_data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1622 2023-04-17 08:15:54.000000 HawaData-0.3.4/test/test_data/test_school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.137390 HawaData-0.3.4/test/test_paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:31.000000 HawaData-0.3.4/test/test_paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      681 2023-03-29 04:15:57.000000 HawaData-0.3.4/test/test_paper/test_health_data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      491 2022-12-02 09:56:11.000000 HawaData-0.3.4/test/test_paper/test_mht_data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.3.4/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.744171 HawaData-0.3.6/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.731392 HawaData-0.3.6/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2200 2023-05-05 08:29:15.000000 HawaData-0.3.6/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      734 2023-05-05 08:29:15.000000 HawaData-0.3.6/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-05 08:29:15.000000 HawaData-0.3.6/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-05 08:29:15.000000 HawaData-0.3.6/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2200 2023-05-05 08:29:15.743780 HawaData-0.3.6/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.3.6/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.731852 HawaData-0.3.6/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.3.6/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.733848 HawaData-0.3.6/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.3.6/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.3.6/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.3.6/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.3.6/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.735604 HawaData-0.3.6/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.3.6/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     8828 2023-05-05 07:06:02.000000 HawaData-0.3.6/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5177 2023-05-05 08:28:22.000000 HawaData-0.3.6/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.3.6/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.3.6/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.736932 HawaData-0.3.6/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.3.6/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.3.6/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.3.6/hawa/data/school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.738409 HawaData-0.3.6/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.3.6/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    23013 2023-05-05 07:06:02.000000 HawaData-0.3.6/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.3.6/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-05 08:29:15.744297 HawaData-0.3.6/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.3.6/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.740317 HawaData-0.3.6/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2022-12-01 08:54:31.000000 HawaData-0.3.6/test/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      654 2022-12-02 04:24:16.000000 HawaData-0.3.6/test/mock.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.741215 HawaData-0.3.6/test/test_common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:19.000000 HawaData-0.3.6/test/test_common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      770 2023-04-13 03:56:08.000000 HawaData-0.3.6/test/test_common/test_common_data.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.742020 HawaData-0.3.6/test/test_data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:40.000000 HawaData-0.3.6/test/test_data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1622 2023-04-17 08:15:54.000000 HawaData-0.3.6/test/test_data/test_school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.743208 HawaData-0.3.6/test/test_paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:31.000000 HawaData-0.3.6/test/test_paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      681 2023-03-29 04:15:57.000000 HawaData-0.3.6/test/test_paper/test_health_data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      491 2022-12-02 09:56:11.000000 HawaData-0.3.6/test/test_paper/test_mht_data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.3.6/test/test_query.py
```

### Comparing `HawaData-0.3.4/HawaData.egg-info/PKG-INFO` & `HawaData-0.3.6/HawaData.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.3.4
+Version: 0.3.6
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -75,7 +75,9 @@
 - 0.2.8 Fix miss grade all
 - 0.2.9 Fix miss grade again
 - 0.3.0 Fix more school when query school
 - 0.3.1 Update replace select *
 - 0.3.2 performance improvement by nickname/username、cronbach_alpha、code_word
 - 0.3.3 performance improvement by grade
 - 0.3.4 up to py3.11
+- 0.3.5 fix engine encoding
+- 0.3.6 update sqlarchemy to 2+
```

### Comparing `HawaData-0.3.4/HawaData.egg-info/SOURCES.txt` & `HawaData-0.3.6/HawaData.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 README.md
 setup.py
 HawaData.egg-info/PKG-INFO
 HawaData.egg-info/SOURCES.txt
 HawaData.egg-info/dependency_links.txt
-HawaData.egg-info/requires.txt
 HawaData.egg-info/top_level.txt
 hawa/__init__.py
 hawa/config.py
 hawa/base/__init__.py
 hawa/base/db.py
 hawa/base/decos.py
 hawa/base/init.py
```

### Comparing `HawaData-0.3.4/PKG-INFO` & `HawaData-0.3.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.3.4
+Version: 0.3.6
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -75,7 +75,9 @@
 - 0.2.8 Fix miss grade all
 - 0.2.9 Fix miss grade again
 - 0.3.0 Fix more school when query school
 - 0.3.1 Update replace select *
 - 0.3.2 performance improvement by nickname/username、cronbach_alpha、code_word
 - 0.3.3 performance improvement by grade
 - 0.3.4 up to py3.11
+- 0.3.5 fix engine encoding
+- 0.3.6 update sqlarchemy to 2+
```

### Comparing `HawaData-0.3.4/README.md` & `HawaData-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.4/hawa/base/db.py` & `HawaData-0.3.6/hawa/base/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 metadata = sqlalchemy.MetaData()
 
 
 @singleton
 class DbUtil:
     _conn = None
     _cursor_conn = None
+    _engine_conn = None
 
     @property
     def conn(self):
         """engine wrapper for pandas.read_sql"""
         if project.COMPLETED:
             try:
                 if not self._conn:
@@ -25,18 +26,24 @@
             except Exception as e:
                 project.logger.info(f"{type(e)=} {e=}")
                 self._conn = self.db_engine
                 return self._conn
         return self.db_engine
 
     @property
+    def engine_conn(self):
+        if not self._engine_conn:
+            self._engine_conn = self.db_engine.connect()
+        return self._engine_conn
+
+    @property
     def db_engine(self):
         database_url = f"{project.DB_MODE}://{project.DB_USER}:{project.DB_PSWD}@{project.DB_HOST}/" \
                        f"{project.DB_NAME}?charset=utf8"
-        engine = sqlalchemy.create_engine(database_url, encoding='utf-8')
+        engine = sqlalchemy.create_engine(database_url)
         return engine
 
     def connect(self):
         return MySQLdb.connect(
             host=project.DB_HOST,
             port=project.DB_PORT,
             user=project.DB_USER,
```

### Comparing `HawaData-0.3.4/hawa/base/init.py` & `HawaData-0.3.6/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.4/hawa/common/data.py` & `HawaData-0.3.6/hawa/common/data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.4/hawa/common/query.py` & `HawaData-0.3.6/hawa/common/query.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from collections import namedtuple
 
 import pandas as pd
+from sqlalchemy import text
 
 from hawa.base.db import DbUtil
 from hawa.base.decos import singleton
 
 
 @singleton
 class DataQuery:
@@ -23,39 +24,39 @@
                 meta_unit = MetaUnit(**data, short_name=data['name'])
             case _:
                 meta_unit = MetaUnit(id=0, name='全国', short_name='全国')
         return meta_unit
 
     def query_schools_all(self):
         sql = f"select id, name, short_name, created from schools;"
-        return pd.read_sql(sql, self.db.conn)
+        return pd.read_sql(text(sql), self.db.engine_conn)
 
     def query_schools_by_ids(self, school_ids: list[int]):
         if len(school_ids) == 0:
             return []
         elif len(school_ids) == 1:
             sql = f"select id, name, short_name, created from schools where id={school_ids[0]};"
         else:
             sql = f"select id, name, short_name, created from schools where id in {tuple(school_ids)};"
-        return pd.read_sql(sql, self.db.conn)
+        return pd.read_sql(text(sql), self.db.engine_conn)
 
     def query_schools_by_startwith(self, startwith: int):
         param_len = len(str(startwith))
         sql = f"select id, name, short_name, created from schools where left(id,{param_len})={startwith};"
-        return pd.read_sql(sql, self.db.conn)
+        return pd.read_sql(text(sql), self.db.engine_conn)
 
     def query_papers(self, test_type: str = '', test_types: list[str] = None):
         """优先 test_types"""
         if test_types:
             sql = f"select id, name, grade, test_type, created from papers where test_type in {tuple(test_types)};"
         elif test_type:
             sql = f"select id, name, grade, test_type, created from papers where test_type='{test_type}';"
         else:
             raise
-        return pd.read_sql(sql, self.db.conn)
+        return pd.read_sql(text(sql), self.db.engine_conn)
 
     def query_cases(
             self, school_ids: list[int], paper_ids: list[int],
             valid_to_start: str, valid_to_end: str,
     ):
         if len(paper_ids) == 0:
             return []
@@ -73,44 +74,44 @@
 
         sql = f"select c.id,c.name,c.valid_from,c.valid_to,c.client_id,c.created," \
               f"c.paper_id,c.is_cleared " \
               f"from cases c " \
               f"inner join case_schools cs on c.id=cs.case_id " \
               f"where  is_cleared=1 and valid_to between '{valid_to_start}' and '{valid_to_end}'" \
               f" {school_sql} {paper_sql};"
-        cases = pd.read_sql(sql, self.db.conn).drop_duplicates(subset=['id'])
+        cases = pd.read_sql(text(sql), self.db.engine_conn).drop_duplicates(subset=['id'])
         return cases
 
     def query_answers(self, case_ids: list[int]):
         answer_cols = "id, student_id, item_id, case_id, answer, score, created, valid"
         if len(case_ids) == 0:
             return []
         elif len(case_ids) == 1:
             sql = f"select {answer_cols} from answers where case_id={case_ids[0]} and valid=1;"
         else:
             sql = f"select {answer_cols} from answers where case_id in {tuple(case_ids)} and valid=1;"
-        answers = pd.read_sql(sql, self.db.conn).drop_duplicates(subset=['case_id', 'student_id', 'item_id'])
+        answers = pd.read_sql(text(sql), self.db.engine_conn).drop_duplicates(subset=['case_id', 'student_id', 'item_id'])
         return answers
 
     def query_students(self, student_ids: list[int]):
         user_cols = "id, username, first_name, last_name, nickname, gender, role, source, created, " \
                     "unit_id, client_id, extra"
         sql = f"select {user_cols} from users where id in {tuple(student_ids)} and length(id)>=18;"
-        students = pd.read_sql(sql, self.db.conn).drop_duplicates(subset=['id'])
+        students = pd.read_sql(text(sql), self.db.engine_conn).drop_duplicates(subset=['id'])
         return students
 
     def query_items(self, item_ids: list[int]):
         item_cols = "id, item_text, choices, item_key, item_type, grade, test_type, pattern, " \
                     "`source`, created"
         sql = f"select {item_cols} from items where id in {tuple(item_ids)};"
-        return pd.read_sql(sql, self.db.conn)
+        return pd.read_sql(text(sql), self.db.engine_conn)
 
     def query_item_codes(self, item_ids: list[int]):
         item_code_sql = f'select ic.item_id,ic.code,ic.category,c.name ' \
                         f'from item_codes ic left join codebook c on ic.code = c.code ' \
                         f'where ic.item_id in {tuple(item_ids)};'
-        item_codes = pd.read_sql(item_code_sql, self.db.conn)
+        item_codes = pd.read_sql(text(item_code_sql), self.db.engine_conn)
         return item_codes
 
     @property
     def conn(self):
         return self.db.conn
```

### Comparing `HawaData-0.3.4/hawa/common/utils.py` & `HawaData-0.3.6/hawa/common/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass, field
 from typing import Optional
 
 import pandas as pd
+from sqlalchemy import text
 
 from hawa.base.db import DbUtil
 from hawa.config import project
 
 
 class Measurement:
     db = DbUtil()
@@ -33,16 +34,16 @@
         return self._get_fields(category='field')
 
     @property
     def dimensions(self):
         return self._get_fields(category='dimension')
 
     def _get_fields(self, category: str):
-        data = pd.read_sql(
-            f"select code, category, name from codebook where category='{category}' and name<>'其他'", self.db.conn)
+        sql = f"select code, category, name from codebook where category='{category}' and name<>'其他'"
+        data = pd.read_sql(text(sql), self.db.engine_conn)
         return data['name'].to_list()
 
     def _get_field_names(self, category: str):
         codes = self._get_fields(category=category)
         return '、'.join(codes[:len(codes) - 1]) + f'与{codes[-1]}'
```

### Comparing `HawaData-0.3.4/hawa/config.py` & `HawaData-0.3.6/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.4/hawa/paper/health.py` & `HawaData-0.3.6/hawa/paper/health.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.4/hawa/paper/mht.py` & `HawaData-0.3.6/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.4/setup.py` & `HawaData-0.3.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,14 @@
     version=text[-1][0],
     author="Steven Wang",
     author_email="brightstar8284@icloud.com",
     description="Use For Unified Hawa Data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/StevenLianaL/HawaData",
-    packages=setuptools.find_packages(exclude=["tests*"]),
-    install_requires=requires,
+    # packages=setuptools.find_packages(exclude=["tests*"]),
+    # install_requires=requires,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
 )
```

### Comparing `HawaData-0.3.4/test/mock.py` & `HawaData-0.3.6/test/mock.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.4/test/test_common/test_common_data.py` & `HawaData-0.3.6/test/test_common/test_common_data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.4/test/test_data/test_school.py` & `HawaData-0.3.6/test/test_data/test_school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.4/test/test_paper/test_health_data.py` & `HawaData-0.3.6/test/test_paper/test_health_data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.4/test/test_query.py` & `HawaData-0.3.6/test/test_query.py`

 * *Files identical despite different names*

