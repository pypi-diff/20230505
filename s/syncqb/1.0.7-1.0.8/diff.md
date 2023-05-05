# Comparing `tmp/syncqb-1.0.7.tar.gz` & `tmp/syncqb-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncqb-1.0.7.tar", last modified: Fri May  5 15:56:00 2023, max compression
+gzip compressed data, was "syncqb-1.0.8.tar", last modified: Fri May  5 16:17:25 2023, max compression
```

## Comparing `syncqb-1.0.7.tar` & `syncqb-1.0.8.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-05 15:56:00.054428 syncqb-1.0.7/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1073 2022-09-12 17:13:14.000000 syncqb-1.0.7/LICENSE
--rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-05-05 15:56:00.054428 syncqb-1.0.7/PKG-INFO
--rw-r--r--   0 jacob     (1000) jacob     (1000)     8642 2023-04-05 20:53:17.000000 syncqb-1.0.7/README.md
--rw-r--r--   0 jacob     (1000) jacob     (1000)      749 2023-05-05 15:49:28.000000 syncqb-1.0.7/pyproject.toml
--rw-r--r--   0 jacob     (1000) jacob     (1000)       38 2023-05-05 15:56:00.054428 syncqb-1.0.7/setup.cfg
--rw-r--r--   0 jacob     (1000) jacob     (1000)       82 2023-04-06 20:44:31.000000 syncqb-1.0.7/setup.py
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-05 15:56:00.043595 syncqb-1.0.7/src/
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-05 15:56:00.043595 syncqb-1.0.7/src/syncqb/
--rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2022-09-12 14:58:01.000000 syncqb-1.0.7/src/syncqb/__init__.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2023-03-29 20:36:22.000000 syncqb-1.0.7/src/syncqb/__init__.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)    17107 2023-05-05 15:50:30.000000 syncqb-1.0.7/src/syncqb/json_quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)    13019 2023-05-05 15:40:29.000000 syncqb-1.0.7/src/syncqb/json_quickbase.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2193 2023-05-05 15:50:43.000000 syncqb-1.0.7/src/syncqb/qb_client.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1665 2023-04-13 17:14:40.000000 syncqb-1.0.7/src/syncqb/qb_client.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1310 2023-04-07 16:31:57.000000 syncqb-1.0.7/src/syncqb/qb_errors.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1046 2023-04-07 14:18:00.000000 syncqb-1.0.7/src/syncqb/qb_errors.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     3274 2023-05-05 15:51:25.000000 syncqb-1.0.7/src/syncqb/quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)      588 2023-04-07 14:18:23.000000 syncqb-1.0.7/src/syncqb/quickbase.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     4205 2023-05-04 21:04:24.000000 syncqb-1.0.7/src/syncqb/test.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)    25524 2023-05-05 15:50:56.000000 syncqb-1.0.7/src/syncqb/xml_quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     8783 2023-04-07 14:18:50.000000 syncqb-1.0.7/src/syncqb/xml_quickbase.pyi
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-05 15:56:00.043595 syncqb-1.0.7/src/syncqb.egg-info/
--rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-05-05 15:56:00.000000 syncqb-1.0.7/src/syncqb.egg-info/PKG-INFO
--rw-r--r--   0 jacob     (1000) jacob     (1000)      576 2023-05-05 15:56:00.000000 syncqb-1.0.7/src/syncqb.egg-info/SOURCES.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)        1 2023-05-05 15:56:00.000000 syncqb-1.0.7/src/syncqb.egg-info/dependency_links.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)       59 2023-05-05 15:56:00.000000 syncqb-1.0.7/src/syncqb.egg-info/entry_points.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)       44 2023-05-05 15:56:00.000000 syncqb-1.0.7/src/syncqb.egg-info/requires.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)        7 2023-05-05 15:56:00.000000 syncqb-1.0.7/src/syncqb.egg-info/top_level.txt
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-05 16:17:25.613499 syncqb-1.0.8/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1073 2022-09-12 17:13:14.000000 syncqb-1.0.8/LICENSE
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-05-05 16:17:25.613499 syncqb-1.0.8/PKG-INFO
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     8642 2023-04-05 20:53:17.000000 syncqb-1.0.8/README.md
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      749 2023-05-05 16:17:09.000000 syncqb-1.0.8/pyproject.toml
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       38 2023-05-05 16:17:25.613499 syncqb-1.0.8/setup.cfg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       82 2023-04-06 20:44:31.000000 syncqb-1.0.8/setup.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-05 16:17:25.602666 syncqb-1.0.8/src/
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-05 16:17:25.613499 syncqb-1.0.8/src/syncqb/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2022-09-12 14:58:01.000000 syncqb-1.0.8/src/syncqb/__init__.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2023-03-29 20:36:22.000000 syncqb-1.0.8/src/syncqb/__init__.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    17111 2023-05-05 16:16:45.000000 syncqb-1.0.8/src/syncqb/json_quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    13019 2023-05-05 15:40:29.000000 syncqb-1.0.8/src/syncqb/json_quickbase.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     2193 2023-05-05 15:50:43.000000 syncqb-1.0.8/src/syncqb/qb_client.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1665 2023-04-13 17:14:40.000000 syncqb-1.0.8/src/syncqb/qb_client.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1310 2023-04-07 16:31:57.000000 syncqb-1.0.8/src/syncqb/qb_errors.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1046 2023-04-07 14:18:00.000000 syncqb-1.0.8/src/syncqb/qb_errors.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     3274 2023-05-05 15:51:25.000000 syncqb-1.0.8/src/syncqb/quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      588 2023-04-07 14:18:23.000000 syncqb-1.0.8/src/syncqb/quickbase.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    25524 2023-05-05 15:50:56.000000 syncqb-1.0.8/src/syncqb/xml_quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     8783 2023-04-07 14:18:50.000000 syncqb-1.0.8/src/syncqb/xml_quickbase.pyi
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-05 16:17:25.613499 syncqb-1.0.8/src/syncqb.egg-info/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-05-05 16:17:25.000000 syncqb-1.0.8/src/syncqb.egg-info/PKG-INFO
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      571 2023-05-05 16:17:25.000000 syncqb-1.0.8/src/syncqb.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        1 2023-05-05 16:17:25.000000 syncqb-1.0.8/src/syncqb.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       59 2023-05-05 16:17:25.000000 syncqb-1.0.8/src/syncqb.egg-info/entry_points.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       44 2023-05-05 16:17:25.000000 syncqb-1.0.8/src/syncqb.egg-info/requires.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        7 2023-05-05 16:17:25.000000 syncqb-1.0.8/src/syncqb.egg-info/top_level.txt
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-05 16:17:25.613499 syncqb-1.0.8/tests/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     4225 2023-05-05 16:16:10.000000 syncqb-1.0.8/tests/test.py
```

### Comparing `syncqb-1.0.7/LICENSE` & `syncqb-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.7/PKG-INFO` & `syncqb-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncqb
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python SDK for quickbase
 Author-email: Jacob Gearhardt <jacob@synctivate.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `syncqb-1.0.7/README.md` & `syncqb-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.7/pyproject.toml` & `syncqb-1.0.8/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0",'requests>=2.25.1','lxml>=4.6.3','chardet>=3.0.4']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "syncqb"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="Jacob Gearhardt", email="jacob@synctivate.com" },
 ]
 description = "A Python SDK for quickbase"
 readme = "README.md"
 license = { file="LICENSE" }
 dependencies = [
```

### Comparing `syncqb-1.0.7/src/syncqb/json_quickbase.py` & `syncqb-1.0.8/src/syncqb/json_quickbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         for index, data in enumerate(response):
             data = self.denest_record(data)
             data = self.replace_empty_values_record(data, default)
             if round_ints:
                 data = self.round_ints_record(data)
             response[index] = data
 
-        return data
+        return response
 
     def _run_report(self, qid, database=None, skip=None, top=None):
         params = {
             'tableId': database or self.database,
             'skip': skip,
             'top': top,
         }
```

### Comparing `syncqb-1.0.7/src/syncqb/json_quickbase.pyi` & `syncqb-1.0.8/src/syncqb/json_quickbase.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.7/src/syncqb/qb_client.py` & `syncqb-1.0.8/src/syncqb/qb_client.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.7/src/syncqb/qb_client.pyi` & `syncqb-1.0.8/src/syncqb/qb_client.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.7/src/syncqb/qb_errors.py` & `syncqb-1.0.8/src/syncqb/qb_errors.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.7/src/syncqb/qb_errors.pyi` & `syncqb-1.0.8/src/syncqb/qb_errors.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.7/src/syncqb/quickbase.py` & `syncqb-1.0.8/src/syncqb/quickbase.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.7/src/syncqb/quickbase.pyi` & `syncqb-1.0.8/src/syncqb/quickbase.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.7/src/syncqb/test.py` & `syncqb-1.0.8/tests/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import qb_client
+from syncqb import qb_client
 from memory_profiler import profile
 # from pprint import pprint
 # from lxml.etree import _Element
 @profile
 def main():
     # table info:
     # database: bnsucj684
@@ -233,33 +233,33 @@
     #     # qid=10, 
     #     columns=[3, 6, 9], 
     #     database='bnsucj684', 
     #     # structured=True,
     #     # qid_custom_headers=True
     # )
     xml_res = 'N/A'
-    json_res = client2.do_query(
-        query=main_asset_query,
-        database=database,
-        columns=columns,
-        # high_volume=True,
-        require_all=True,
-    )
     # json_res = client2.do_query(
-    #     query='{3.EX.128}',
-    #     # qid=10,
-    #     columns=[3, 6, 9], 
-    #     database='bnsucj684',
+    #     query=main_asset_query,
+    #     database=database,
+    #     columns=columns,
+    #     # high_volume=True,
+    #     require_all=True,
     # )
+    json_res = client2.do_query(
+        query='{3.EX.128}',
+        # qid=10,
+        columns=[3, 6, 9], 
+        database='bnsucj684',
+    )
     # json_res = 'N/A'
 
     # print('xml_res:', xml_res)
-    # for record in json_res:
-    #     print(record)
-    print('json_res:')
+    for record in json_res:
+        print(record)
+    print('json_res:', json_res)
     
 
 
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `syncqb-1.0.7/src/syncqb/xml_quickbase.py` & `syncqb-1.0.8/src/syncqb/xml_quickbase.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.7/src/syncqb/xml_quickbase.pyi` & `syncqb-1.0.8/src/syncqb/xml_quickbase.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.7/src/syncqb.egg-info/PKG-INFO` & `syncqb-1.0.8/src/syncqb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncqb
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python SDK for quickbase
 Author-email: Jacob Gearhardt <jacob@synctivate.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `syncqb-1.0.7/src/syncqb.egg-info/SOURCES.txt` & `syncqb-1.0.8/src/syncqb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 src/syncqb/json_quickbase.pyi
 src/syncqb/qb_client.py
 src/syncqb/qb_client.pyi
 src/syncqb/qb_errors.py
 src/syncqb/qb_errors.pyi
 src/syncqb/quickbase.py
 src/syncqb/quickbase.pyi
-src/syncqb/test.py
 src/syncqb/xml_quickbase.py
 src/syncqb/xml_quickbase.pyi
 src/syncqb.egg-info/PKG-INFO
 src/syncqb.egg-info/SOURCES.txt
 src/syncqb.egg-info/dependency_links.txt
 src/syncqb.egg-info/entry_points.txt
 src/syncqb.egg-info/requires.txt
-src/syncqb.egg-info/top_level.txt
+src/syncqb.egg-info/top_level.txt
+tests/test.py
```

