# Comparing `tmp/HawaData-0.3.6.tar.gz` & `tmp/HawaData-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.3.6.tar", last modified: Fri May  5 08:29:15 2023, max compression
+gzip compressed data, was "HawaData-0.3.7.tar", last modified: Fri May  5 09:08:35 2023, max compression
```

## Comparing `HawaData-0.3.6.tar` & `HawaData-0.3.7.tar`

### file list

```diff
@@ -1,45 +1,33 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.744171 HawaData-0.3.6/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.731392 HawaData-0.3.6/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2200 2023-05-05 08:29:15.000000 HawaData-0.3.6/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      734 2023-05-05 08:29:15.000000 HawaData-0.3.6/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-05 08:29:15.000000 HawaData-0.3.6/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-05 08:29:15.000000 HawaData-0.3.6/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     2200 2023-05-05 08:29:15.743780 HawaData-0.3.6/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.3.6/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.731852 HawaData-0.3.6/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.3.6/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.733848 HawaData-0.3.6/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.3.6/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.3.6/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.3.6/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.3.6/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.735604 HawaData-0.3.6/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.3.6/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     8828 2023-05-05 07:06:02.000000 HawaData-0.3.6/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5177 2023-05-05 08:28:22.000000 HawaData-0.3.6/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.3.6/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.3.6/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.736932 HawaData-0.3.6/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.3.6/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.3.6/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.3.6/hawa/data/school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.738409 HawaData-0.3.6/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.3.6/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    23013 2023-05-05 07:06:02.000000 HawaData-0.3.6/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.3.6/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-05 08:29:15.744297 HawaData-0.3.6/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.3.6/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.740317 HawaData-0.3.6/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2022-12-01 08:54:31.000000 HawaData-0.3.6/test/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      654 2022-12-02 04:24:16.000000 HawaData-0.3.6/test/mock.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.741215 HawaData-0.3.6/test/test_common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:19.000000 HawaData-0.3.6/test/test_common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      770 2023-04-13 03:56:08.000000 HawaData-0.3.6/test/test_common/test_common_data.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.742020 HawaData-0.3.6/test/test_data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:40.000000 HawaData-0.3.6/test/test_data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1622 2023-04-17 08:15:54.000000 HawaData-0.3.6/test/test_data/test_school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 08:29:15.743208 HawaData-0.3.6/test/test_paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:31.000000 HawaData-0.3.6/test/test_paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      681 2023-03-29 04:15:57.000000 HawaData-0.3.6/test/test_paper/test_health_data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      491 2022-12-02 09:56:11.000000 HawaData-0.3.6/test/test_paper/test_mht_data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.3.6/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:08:35.641916 HawaData-0.3.7/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:08:35.634363 HawaData-0.3.7/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2228 2023-05-05 09:08:35.000000 HawaData-0.3.7/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      484 2023-05-05 09:08:35.000000 HawaData-0.3.7/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-05 09:08:35.000000 HawaData-0.3.7/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-05 09:08:35.000000 HawaData-0.3.7/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2228 2023-05-05 09:08:35.641511 HawaData-0.3.7/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.3.7/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:08:35.634875 HawaData-0.3.7/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.3.7/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:08:35.636550 HawaData-0.3.7/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.3.7/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.3.7/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.3.7/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.3.7/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:08:35.638245 HawaData-0.3.7/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.3.7/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     8828 2023-05-05 07:06:02.000000 HawaData-0.3.7/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5177 2023-05-05 08:28:22.000000 HawaData-0.3.7/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.3.7/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.3.7/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:08:35.639561 HawaData-0.3.7/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.3.7/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.3.7/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.3.7/hawa/data/school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:08:35.640746 HawaData-0.3.7/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.3.7/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    22995 2023-05-05 09:08:17.000000 HawaData-0.3.7/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.3.7/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-05 09:08:35.642011 HawaData-0.3.7/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.3.7/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:08:35.641049 HawaData-0.3.7/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.3.7/test/test_query.py
```

### Comparing `HawaData-0.3.6/HawaData.egg-info/PKG-INFO` & `HawaData-0.3.7/HawaData.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.3.6
+Version: 0.3.7
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -77,7 +77,8 @@
 - 0.3.0 Fix more school when query school
 - 0.3.1 Update replace select *
 - 0.3.2 performance improvement by nickname/username、cronbach_alpha、code_word
 - 0.3.3 performance improvement by grade
 - 0.3.4 up to py3.11
 - 0.3.5 fix engine encoding
 - 0.3.6 update sqlarchemy to 2+
+- 0.3.7 update pandas to 2+
```

### Comparing `HawaData-0.3.6/PKG-INFO` & `HawaData-0.3.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.3.6
+Version: 0.3.7
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -77,7 +77,8 @@
 - 0.3.0 Fix more school when query school
 - 0.3.1 Update replace select *
 - 0.3.2 performance improvement by nickname/username、cronbach_alpha、code_word
 - 0.3.3 performance improvement by grade
 - 0.3.4 up to py3.11
 - 0.3.5 fix engine encoding
 - 0.3.6 update sqlarchemy to 2+
+- 0.3.7 update pandas to 2+
```

### Comparing `HawaData-0.3.6/README.md` & `HawaData-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.6/hawa/base/db.py` & `HawaData-0.3.7/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.6/hawa/base/init.py` & `HawaData-0.3.7/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.6/hawa/common/data.py` & `HawaData-0.3.7/hawa/common/data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.6/hawa/common/query.py` & `HawaData-0.3.7/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.6/hawa/common/utils.py` & `HawaData-0.3.7/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.6/hawa/config.py` & `HawaData-0.3.7/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.6/hawa/paper/health.py` & `HawaData-0.3.7/hawa/paper/health.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     def _to_count_f_case_gender_counts(self):
         """单年级，各班级性别数据；多年级，各年级性别数据。"""
         ans = self.final_answers.drop_duplicates(subset=['student_id'])
         data = ans.loc[:, ['grade', 'cls', 'gender', 'student_id']]
         # 年级 班级 男生数 女生数 总人数
         # 班级 男生数 女生数 总人数
         records = []
-        for grade, grade_group in data.groupby(by=['grade']):
+        for grade, grade_group in data.groupby(by='grade'):
             for cls, cls_group in grade_group.groupby('cls'):
                 grade_cls = Munch(grade=grade, cls=cls)
                 cls_total = Munch(total=len(cls_group))
                 cls_gender = cls_group.gender.value_counts().to_dict()
                 records.append(grade_cls | cls_total | cls_gender)
             grade_total = Munch(total=len(grade_group))
             grade_gender = grade_group.gender.value_counts().to_dict()
@@ -207,17 +207,16 @@
         for grade in self.grade.grades:
             base: pd.DataFrame = scores.loc[scores.grade == grade, :]
             base_dimensions = base.loc[base.category == 'dimension', ['code', 'total']]
             base_fields = base.loc[base.category == 'field', ['code', 'total']]
 
             dimensions = self._count_df_reverse(first_col='code', second_col='total', data=base_dimensions)
             fields = self._count_df_reverse(first_col='code', second_col='total', data=base_fields)
-
-            a = base.loc[base.category == 'field', ['code', 'F']].mean().mean()
-            b = base.loc[base.category == 'field', ['code', 'M']].mean().mean()
+            a = base.loc[base.category == 'field', ['F']].mean().mean()
+            b = base.loc[base.category == 'field', ['M']].mean().mean()
             records[grade] = {
                 'dimension': dimensions, 'field': fields,
                 'cond': self.count_cond(a, b)
             }
         self.grade_code_score = records
 
     def _to_count_n_compare_grade_year_school(self):
@@ -334,15 +333,15 @@
     def gender_count(self) -> Munch:
         r = self.students.gender.value_counts()
         return Munch({'M': 0, 'F': 0} | r.to_dict())
 
     # 工具函数
 
     def _count_df_reverse(self, first_col: str, second_col: str, data: pd.DataFrame):
-        base = data.to_dict(orient='record')
+        base = data.to_dict(orient='records')
         middle = {d[first_col]: d[second_col] / 100 for d in base}
         reverse_middle = {v: k for k, v in middle.items()}
         res = [(self._retain_prec(k), reverse_middle[k]) for k in sorted(reverse_middle.keys(), reverse=True)]
         return res
 
     def count_cond(self, a: float, b: float):
         if a == b:
```

### Comparing `HawaData-0.3.6/hawa/paper/mht.py` & `HawaData-0.3.7/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.6/setup.py` & `HawaData-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.6/test/test_query.py` & `HawaData-0.3.7/test/test_query.py`

 * *Files identical despite different names*

