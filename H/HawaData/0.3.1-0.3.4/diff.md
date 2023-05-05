# Comparing `tmp/HawaData-0.3.1.tar.gz` & `tmp/HawaData-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.3.1.tar", last modified: Tue Apr 25 10:02:22 2023, max compression
+gzip compressed data, was "HawaData-0.3.4.tar", last modified: Fri May  5 07:43:51 2023, max compression
```

## Comparing `HawaData-0.3.1.tar` & `HawaData-0.3.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.205297 HawaData-0.3.1/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.192860 HawaData-0.3.1/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     1996 2023-04-25 10:02:22.000000 HawaData-0.3.1/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      765 2023-04-25 10:02:22.000000 HawaData-0.3.1/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-04-25 10:02:22.000000 HawaData-0.3.1/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)      257 2023-04-25 10:02:22.000000 HawaData-0.3.1/HawaData.egg-info/requires.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)       10 2023-04-25 10:02:22.000000 HawaData-0.3.1/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     1996 2023-04-25 10:02:22.205038 HawaData-0.3.1/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.3.1/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.193389 HawaData-0.3.1/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.3.1/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.195282 HawaData-0.3.1/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.3.1/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2842 2022-12-11 02:48:15.000000 HawaData-0.3.1/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.3.1/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.3.1/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.197136 HawaData-0.3.1/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.3.1/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     8767 2023-04-17 08:29:21.000000 HawaData-0.3.1/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5032 2023-04-25 09:59:36.000000 HawaData-0.3.1/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2710 2023-04-25 09:04:45.000000 HawaData-0.3.1/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.3.1/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.198620 HawaData-0.3.1/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.3.1/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.3.1/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.3.1/hawa/data/school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.200247 HawaData-0.3.1/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.3.1/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    22989 2023-04-13 07:01:46.000000 HawaData-0.3.1/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5252 2022-12-08 10:47:44.000000 HawaData-0.3.1/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-04-25 10:02:22.205375 HawaData-0.3.1/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      875 2022-12-02 07:10:09.000000 HawaData-0.3.1/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.201775 HawaData-0.3.1/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2022-12-01 08:54:31.000000 HawaData-0.3.1/test/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      654 2022-12-02 04:24:16.000000 HawaData-0.3.1/test/mock.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.202465 HawaData-0.3.1/test/test_common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:19.000000 HawaData-0.3.1/test/test_common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      770 2023-04-13 03:56:08.000000 HawaData-0.3.1/test/test_common/test_common_data.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.203296 HawaData-0.3.1/test/test_data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:40.000000 HawaData-0.3.1/test/test_data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1622 2023-04-17 08:15:54.000000 HawaData-0.3.1/test/test_data/test_school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.204477 HawaData-0.3.1/test/test_paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:31.000000 HawaData-0.3.1/test/test_paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      681 2023-03-29 04:15:57.000000 HawaData-0.3.1/test/test_paper/test_health_data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      491 2022-12-02 09:56:11.000000 HawaData-0.3.1/test/test_paper/test_mht_data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.3.1/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.138455 HawaData-0.3.4/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.125710 HawaData-0.3.4/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2140 2023-05-05 07:43:51.000000 HawaData-0.3.4/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      765 2023-05-05 07:43:51.000000 HawaData-0.3.4/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-05 07:43:51.000000 HawaData-0.3.4/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)      141 2023-05-05 07:43:51.000000 HawaData-0.3.4/HawaData.egg-info/requires.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)       10 2023-05-05 07:43:51.000000 HawaData-0.3.4/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2140 2023-05-05 07:43:51.138052 HawaData-0.3.4/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.3.4/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.126475 HawaData-0.3.4/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.3.4/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.128938 HawaData-0.3.4/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.3.4/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2842 2022-12-11 02:48:15.000000 HawaData-0.3.4/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.3.4/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.3.4/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.130755 HawaData-0.3.4/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.3.4/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     8828 2023-05-05 07:06:02.000000 HawaData-0.3.4/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5032 2023-04-25 09:59:36.000000 HawaData-0.3.4/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2738 2023-05-05 07:06:32.000000 HawaData-0.3.4/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.3.4/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.131959 HawaData-0.3.4/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.3.4/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.3.4/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.3.4/hawa/data/school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.133183 HawaData-0.3.4/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.3.4/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    23013 2023-05-05 07:06:02.000000 HawaData-0.3.4/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.3.4/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-05 07:43:51.138584 HawaData-0.3.4/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      875 2022-12-02 07:10:09.000000 HawaData-0.3.4/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.134795 HawaData-0.3.4/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2022-12-01 08:54:31.000000 HawaData-0.3.4/test/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      654 2022-12-02 04:24:16.000000 HawaData-0.3.4/test/mock.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.135466 HawaData-0.3.4/test/test_common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:19.000000 HawaData-0.3.4/test/test_common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      770 2023-04-13 03:56:08.000000 HawaData-0.3.4/test/test_common/test_common_data.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.136250 HawaData-0.3.4/test/test_data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:40.000000 HawaData-0.3.4/test/test_data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1622 2023-04-17 08:15:54.000000 HawaData-0.3.4/test/test_data/test_school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 07:43:51.137390 HawaData-0.3.4/test/test_paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:31.000000 HawaData-0.3.4/test/test_paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      681 2023-03-29 04:15:57.000000 HawaData-0.3.4/test/test_paper/test_health_data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      491 2022-12-02 09:56:11.000000 HawaData-0.3.4/test/test_paper/test_mht_data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.3.4/test/test_query.py
```

### Comparing `HawaData-0.3.1/HawaData.egg-info/PKG-INFO` & `HawaData-0.3.4/HawaData.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.3.1
+Version: 0.3.4
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -72,7 +72,10 @@
 - 0.2.5 Filter users when length id <18 true
 - 0.2.6 Fix rank dis
 - 0.2.7 Fix miss grade
 - 0.2.8 Fix miss grade all
 - 0.2.9 Fix miss grade again
 - 0.3.0 Fix more school when query school
 - 0.3.1 Update replace select *
+- 0.3.2 performance improvement by nickname/username、cronbach_alpha、code_word
+- 0.3.3 performance improvement by grade
+- 0.3.4 up to py3.11
```

### Comparing `HawaData-0.3.1/HawaData.egg-info/SOURCES.txt` & `HawaData-0.3.4/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.1/PKG-INFO` & `HawaData-0.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.3.1
+Version: 0.3.4
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -72,7 +72,10 @@
 - 0.2.5 Filter users when length id <18 true
 - 0.2.6 Fix rank dis
 - 0.2.7 Fix miss grade
 - 0.2.8 Fix miss grade all
 - 0.2.9 Fix miss grade again
 - 0.3.0 Fix more school when query school
 - 0.3.1 Update replace select *
+- 0.3.2 performance improvement by nickname/username、cronbach_alpha、code_word
+- 0.3.3 performance improvement by grade
+- 0.3.4 up to py3.11
```

### Comparing `HawaData-0.3.1/README.md` & `HawaData-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.1/hawa/base/db.py` & `HawaData-0.3.4/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.1/hawa/base/init.py` & `HawaData-0.3.4/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.1/hawa/common/data.py` & `HawaData-0.3.4/hawa/common/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,40 +42,40 @@
     db: ClassVar[DbUtil] = None
     redis: ClassVar[RedisUtil] = None
     query: ClassVar[DataQuery] = None
 
     # 原始数据
 
     school_ids: list[int] = field(default_factory=list)
-    schools: pd.DataFrame = pd.DataFrame()
+    schools: pd.DataFrame = field(default_factory=pd.DataFrame)
 
-    cases: pd.DataFrame = pd.DataFrame()
+    cases: pd.DataFrame = field(default_factory=pd.DataFrame)
     case_ids: list[int] = field(default_factory=list)
 
-    answers: pd.DataFrame = pd.DataFrame()
+    answers: pd.DataFrame = field(default_factory=pd.DataFrame)
 
-    students: pd.DataFrame = pd.DataFrame()
+    students: pd.DataFrame = field(default_factory=pd.DataFrame)
     student_ids: list[int] = field(default_factory=list)
     student_count: Optional[int] = None
 
     item_ids: Optional[set[int]] = None
     items: Optional[pd.DataFrame] = None
 
     # 辅助工具
     grade_util: Optional[GradeData] = None
     case_util: Optional[CaseData] = None
     measurement = Measurement()
 
     # 计算数据
-    final_answers: pd.DataFrame = pd.DataFrame()
-    final_scores: pd.DataFrame = pd.DataFrame()
+    final_answers: pd.DataFrame = field(default_factory=pd.DataFrame)
+    final_scores: pd.DataFrame = field(default_factory=pd.DataFrame)
 
     # 去年全国数据
     last_year = None
-    last_year_code_scores: Optional[pd.DataFrame] = pd.DataFrame()
+    last_year_code_scores: Optional[pd.DataFrame] = field(default_factory=pd.DataFrame)
 
     def __post_init__(self):
         # 初始化数据
         init_functions = [i for i in dir(self) if i.startswith('_to_init_')]
         for func in init_functions:
             getattr(self, func)()
 
@@ -144,45 +144,44 @@
         project.logger.debug(f'items: {len(self.items)}')
 
     def _to_build_helper(self):
         self.grade = GradeData(case_ids=self.case_ids)
         self.case = CaseData(cases=self.cases)
 
     def _to_count_a_final_answers(self):
-        items = {}
+        items = {k: {} for k in self.code_word_list}
         item_codes = self.query.query_item_codes(self.item_ids)
+        # code-dimension/field  ~  item_id  ~ code   name
         project.logger.debug(f"{self.code_word_list=}")
-        for item_id, codes in item_codes.groupby('item_id'):
-            items[item_id] = [i for i in codes.to_dict(orient='records')
-                              if i['category'] in self.code_word_list]
+        for (item_id, category), codes in item_codes.groupby(['item_id', 'category']):
+            if category in self.code_word_list:
+                for _, code_data in codes.iterrows():
+                    items[category][item_id] = code_data['name']
 
         data = pd.merge(
-            self.answers, self.students.loc[:, ['id', 'gender', 'first_name', 'last_name']],
+            self.answers, self.students.loc[:, ['id', 'gender', 'nickname']],
             left_on='student_id', right_on='id'
         )
         project.logger.debug(f"ans merge students {len(data)}")
         # inner 时，final_answers 和 answers 数目不等：final_answers 过滤掉了 没有 code_word_list（维度领域或其他）的题目
         # outer 时，数目相等，不过滤任何题目
         data = pd.merge(data, item_codes, left_on='item_id', right_on='item_id', how='inner')
 
         data['cls'] = data['id_y'].apply(lambda x: int(str(x)[13:15]))
-        data['grade'] = data['case_id'].apply(lambda x: int(str(x)[-2:]))
-        data['username'] = data.apply(lambda x: f"{x.last_name}{x.first_name}", axis=1)
+        data['grade'] = data['case_id'].apply(lambda x: x % 100)
+        data['username'] = data['nickname']
         for code_word in self.code_word_list:
-            data[code_word] = data.item_id.apply(self._count_field, args=(code_word, items))
+            data[code_word] = data.item_id.apply(lambda x: items[code_word][x])
         self.final_answers = data.drop_duplicates(subset=['case_id', 'student_id', 'item_id'])
         project.logger.debug(f'final_answers: {len(self.final_answers)}')
 
     def _to_count_b_final_scores(self):
         self.final_scores = self.count_final_score(answers=self.final_answers)
         project.logger.debug(f'final_scores: {len(self.final_scores)}')
 
-    def _count_field(self, item_id: int, code: str, items: dict):
-        return [i for i in items[item_id] if i['category'] == code][0]['name']
-
     @staticmethod
     def count_level(score, mode: str = 'f'):
         assert mode in ('f', 'r'), 'only support feedback or report'
         if score >= 90:
             a = 'A'
         elif score >= 80:
             a = 'B'
```

### Comparing `HawaData-0.3.1/hawa/common/query.py` & `HawaData-0.3.4/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.1/hawa/common/utils.py` & `HawaData-0.3.4/hawa/common/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Optional
 
 import pandas as pd
 
-from hawa.config import project
 from hawa.base.db import DbUtil
+from hawa.config import project
 
 
 class Measurement:
     db = DbUtil()
 
     @property
     def level_names(self):
@@ -44,15 +44,15 @@
     def _get_field_names(self, category: str):
         codes = self._get_fields(category=category)
         return '、'.join(codes[:len(codes) - 1]) + f'与{codes[-1]}'
 
 
 @dataclass
 class CaseData:
-    cases: pd.DataFrame = pd.DataFrame()
+    cases: pd.DataFrame = field(default_factory=pd.DataFrame)
 
     @property
     def join_date(self):
         valid_from = self.cases['valid_from'].min()
         valid_to = self.cases['valid_to'].max()
         if (valid_from.month, valid_from.day) == (valid_to.month, valid_to.day):
             join_date = f"参测日期：{valid_from:%Y年%m月%d日}"
```

### Comparing `HawaData-0.3.1/hawa/config.py` & `HawaData-0.3.4/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.1/hawa/paper/health.py` & `HawaData-0.3.4/hawa/paper/health.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import random
 from collections import defaultdict
 from dataclasses import dataclass, field
 from typing import Union, Set
 
 import pandas as pd
 from munch import Munch
+from pingouin import cronbach_alpha
 
 from hawa.common.data import CommonData
 from hawa.config import project
 
 
 @dataclass
 class HealthData(CommonData):
@@ -25,15 +26,15 @@
         else:
             return text.replace('还', '')
 
 
 @dataclass
 class HealthReportData(HealthData):
     # 计算数据
-    code_scores: pd.DataFrame = pd.DataFrame()
+    code_scores: pd.DataFrame = field(default_factory=pd.DataFrame)
     summary_scores: dict = field(default_factory=dict)
     grade_good_bad = None  # 优势 优先关注点
 
     grade_rank_dis = None  # 年级、性别、水平学生分布占比
     grade_reverse_rank_dis = None  # 占比由高到低的年级分布水平
     grade_gender_distribution = None
     grade_score = None  # 年级最高、最低、平均分
@@ -133,21 +134,20 @@
             records['cls'] = records.apply(self._count_cls, axis=1)
         else:
             records['grade'] = records.grade.apply(lambda x: f"{project.grade_simple[x]}年级")
             records = records.loc[records.cls == 0, :]
         self.case_gender_counts = records.to_dict(orient='records')
 
     def _to_count_g_cronbach_alpha(self):
-        import pingouin as pg
         cols = ['student_id', 'item_id', 'score']
         res = []
         for grade, group in self.final_answers.groupby('grade'):
             base = group.loc[:, cols]
             data = pd.pivot_table(base, index='item_id', columns='student_id', values='score')
-            c: tuple = pg.cronbach_alpha(data)
+            c: tuple = cronbach_alpha(data)
             res.append(c[0])
         self.cronbach_alpha = [round(i, 3) for i in res]
 
     def _to_count_h_grade_gender_distribution(self):
         """年级性别分布"""
         data = self.case_gender_counts
         records = {}
```

### Comparing `HawaData-0.3.1/hawa/paper/mht.py` & `HawaData-0.3.4/hawa/paper/mht.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     grade_sub_scale_score: dict = field(default_factory=dict)
     grade_special_students: dict = field(default_factory=dict)
 
     # 计算数据2
     invalid_student_count: int = 0
     unused_student_count: int = 0
     unused_student_ids: list[int] = field(default_factory=list)
-    mht_final_answers: pd.DataFrame = pd.DataFrame()
+    mht_final_answers: pd.DataFrame = field(default_factory=pd.DataFrame)
 
     def _to_count_a_final_answers(self):
         super()._to_count_a_final_answers()
         old_answers = self.final_answers
         old_answers['score'] = old_answers['score'].astype(int)
 
         # 去除具备社会期许效应的学生
```

### Comparing `HawaData-0.3.1/setup.py` & `HawaData-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.1/test/mock.py` & `HawaData-0.3.4/test/mock.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.1/test/test_common/test_common_data.py` & `HawaData-0.3.4/test/test_common/test_common_data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.1/test/test_data/test_school.py` & `HawaData-0.3.4/test/test_data/test_school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.1/test/test_paper/test_health_data.py` & `HawaData-0.3.4/test/test_paper/test_health_data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.1/test/test_query.py` & `HawaData-0.3.4/test/test_query.py`

 * *Files identical despite different names*

