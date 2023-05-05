# Comparing `tmp/HawaData-0.3.7.tar.gz` & `tmp/HawaData-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.3.7.tar", last modified: Fri May  5 09:08:35 2023, max compression
+gzip compressed data, was "HawaData-0.3.8.tar", last modified: Fri May  5 09:22:50 2023, max compression
```

## Comparing `HawaData-0.3.7.tar` & `HawaData-0.3.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:08:35.641916 HawaData-0.3.7/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:08:35.634363 HawaData-0.3.7/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2228 2023-05-05 09:08:35.000000 HawaData-0.3.7/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      484 2023-05-05 09:08:35.000000 HawaData-0.3.7/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-05 09:08:35.000000 HawaData-0.3.7/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-05 09:08:35.000000 HawaData-0.3.7/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     2228 2023-05-05 09:08:35.641511 HawaData-0.3.7/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.3.7/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:08:35.634875 HawaData-0.3.7/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.3.7/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:08:35.636550 HawaData-0.3.7/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.3.7/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.3.7/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.3.7/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.3.7/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:08:35.638245 HawaData-0.3.7/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.3.7/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     8828 2023-05-05 07:06:02.000000 HawaData-0.3.7/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5177 2023-05-05 08:28:22.000000 HawaData-0.3.7/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.3.7/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.3.7/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:08:35.639561 HawaData-0.3.7/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.3.7/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.3.7/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.3.7/hawa/data/school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:08:35.640746 HawaData-0.3.7/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.3.7/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    22995 2023-05-05 09:08:17.000000 HawaData-0.3.7/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.3.7/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-05 09:08:35.642011 HawaData-0.3.7/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.3.7/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:08:35.641049 HawaData-0.3.7/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.3.7/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:22:50.280458 HawaData-0.3.8/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:22:50.275068 HawaData-0.3.8/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2250 2023-05-05 09:22:50.000000 HawaData-0.3.8/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      484 2023-05-05 09:22:50.000000 HawaData-0.3.8/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-05 09:22:50.000000 HawaData-0.3.8/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-05 09:22:50.000000 HawaData-0.3.8/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2250 2023-05-05 09:22:50.280193 HawaData-0.3.8/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.3.8/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:22:50.275602 HawaData-0.3.8/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.3.8/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:22:50.276708 HawaData-0.3.8/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.3.8/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.3.8/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.3.8/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.3.8/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:22:50.277807 HawaData-0.3.8/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.3.8/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     8901 2023-05-05 09:20:15.000000 HawaData-0.3.8/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5177 2023-05-05 08:28:22.000000 HawaData-0.3.8/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.3.8/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.3.8/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:22:50.278714 HawaData-0.3.8/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.3.8/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.3.8/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.3.8/hawa/data/school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:22:50.279570 HawaData-0.3.8/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.3.8/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    22995 2023-05-05 09:08:17.000000 HawaData-0.3.8/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.3.8/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-05 09:22:50.280532 HawaData-0.3.8/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.3.8/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-05 09:22:50.279853 HawaData-0.3.8/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.3.8/test/test_query.py
```

### Comparing `HawaData-0.3.7/HawaData.egg-info/PKG-INFO` & `HawaData-0.3.8/HawaData.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.3.7
+Version: 0.3.8
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -78,7 +78,8 @@
 - 0.3.1 Update replace select *
 - 0.3.2 performance improvement by nickname/username、cronbach_alpha、code_word
 - 0.3.3 performance improvement by grade
 - 0.3.4 up to py3.11
 - 0.3.5 fix engine encoding
 - 0.3.6 update sqlarchemy to 2+
 - 0.3.7 update pandas to 2+
+- 0.3.8 fix loss data
```

### Comparing `HawaData-0.3.7/PKG-INFO` & `HawaData-0.3.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.3.7
+Version: 0.3.8
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -78,7 +78,8 @@
 - 0.3.1 Update replace select *
 - 0.3.2 performance improvement by nickname/username、cronbach_alpha、code_word
 - 0.3.3 performance improvement by grade
 - 0.3.4 up to py3.11
 - 0.3.5 fix engine encoding
 - 0.3.6 update sqlarchemy to 2+
 - 0.3.7 update pandas to 2+
+- 0.3.8 fix loss data
```

### Comparing `HawaData-0.3.7/README.md` & `HawaData-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.7/hawa/base/db.py` & `HawaData-0.3.8/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.7/hawa/base/init.py` & `HawaData-0.3.8/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.7/hawa/common/data.py` & `HawaData-0.3.8/hawa/common/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,16 +210,19 @@
     def get_last_year_miss(self, grade: int):
         key = f'{project.REDIS_PREFIX}{self.last_year_num}:data'
         data = json.loads(self.redis.conn.get(key))
         try:
             grade_data = data[str(grade)]
         except KeyError:
             temp_key = f'{project.REDIS_PREFIX}{self.last_year_num - 1}:data'
-            temp_data = json.loads(self.redis.conn.get(temp_key))
-            try:
+            print(temp_key,'tk')
+            temp_cache_data=self.redis.conn.get(temp_key)
+            if temp_cache_data:
+                temp_data = json.loads(temp_cache_data)
                 grade_data = temp_data[str(grade - 1)]
-            except KeyError:
-                grade_data = temp_data[str(grade - 3)]
+            else:
+                grade_data = data[str(3)]
+
         grade_data['people']['grade'] = f"{grade}年级"
         for k, v in grade_data['code'].items():
             grade_data['code'][k]['grade'] = grade
         return grade_data
```

### Comparing `HawaData-0.3.7/hawa/common/query.py` & `HawaData-0.3.8/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.7/hawa/common/utils.py` & `HawaData-0.3.8/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.7/hawa/config.py` & `HawaData-0.3.8/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.7/hawa/paper/health.py` & `HawaData-0.3.8/hawa/paper/health.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.7/hawa/paper/mht.py` & `HawaData-0.3.8/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.7/setup.py` & `HawaData-0.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.7/test/test_query.py` & `HawaData-0.3.8/test/test_query.py`

 * *Files identical despite different names*

