# Comparing `tmp/syncqb-1.0.6.tar.gz` & `tmp/syncqb-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncqb-1.0.6.tar", last modified: Mon May  1 15:34:48 2023, max compression
+gzip compressed data, was "syncqb-1.0.7.tar", last modified: Fri May  5 15:56:00 2023, max compression
```

## Comparing `syncqb-1.0.6.tar` & `syncqb-1.0.7.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-01 15:34:48.937323 syncqb-1.0.6/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1073 2022-09-12 17:13:14.000000 syncqb-1.0.6/LICENSE
--rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-05-01 15:34:48.937323 syncqb-1.0.6/PKG-INFO
--rw-r--r--   0 jacob     (1000) jacob     (1000)     8642 2023-04-05 20:53:17.000000 syncqb-1.0.6/README.md
--rw-r--r--   0 jacob     (1000) jacob     (1000)      749 2023-05-01 15:34:26.000000 syncqb-1.0.6/pyproject.toml
--rw-r--r--   0 jacob     (1000) jacob     (1000)       38 2023-05-01 15:34:48.937323 syncqb-1.0.6/setup.cfg
--rw-r--r--   0 jacob     (1000) jacob     (1000)       82 2023-04-06 20:44:31.000000 syncqb-1.0.6/setup.py
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-01 15:34:48.915656 syncqb-1.0.6/src/
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-01 15:34:48.926489 syncqb-1.0.6/src/syncqb/
--rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2022-09-12 14:58:01.000000 syncqb-1.0.6/src/syncqb/__init__.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2023-03-29 20:36:22.000000 syncqb-1.0.6/src/syncqb/__init__.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)    16499 2023-05-01 15:30:52.000000 syncqb-1.0.6/src/syncqb/json_quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)    11395 2023-04-21 14:13:40.000000 syncqb-1.0.6/src/syncqb/json_quickbase.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2193 2023-05-01 15:30:51.000000 syncqb-1.0.6/src/syncqb/qb_client.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1665 2023-04-13 17:14:40.000000 syncqb-1.0.6/src/syncqb/qb_client.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1310 2023-04-07 16:31:57.000000 syncqb-1.0.6/src/syncqb/qb_errors.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1046 2023-04-07 14:18:00.000000 syncqb-1.0.6/src/syncqb/qb_errors.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     3022 2023-05-01 15:30:50.000000 syncqb-1.0.6/src/syncqb/quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)      588 2023-04-07 14:18:23.000000 syncqb-1.0.6/src/syncqb/quickbase.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)    25524 2023-05-01 15:30:49.000000 syncqb-1.0.6/src/syncqb/xml_quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     8783 2023-04-07 14:18:50.000000 syncqb-1.0.6/src/syncqb/xml_quickbase.pyi
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-01 15:34:48.937323 syncqb-1.0.6/src/syncqb.egg-info/
--rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-05-01 15:34:48.000000 syncqb-1.0.6/src/syncqb.egg-info/PKG-INFO
--rw-r--r--   0 jacob     (1000) jacob     (1000)      571 2023-05-01 15:34:48.000000 syncqb-1.0.6/src/syncqb.egg-info/SOURCES.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)        1 2023-05-01 15:34:48.000000 syncqb-1.0.6/src/syncqb.egg-info/dependency_links.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)       59 2023-05-01 15:34:48.000000 syncqb-1.0.6/src/syncqb.egg-info/entry_points.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)       44 2023-05-01 15:34:48.000000 syncqb-1.0.6/src/syncqb.egg-info/requires.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)        7 2023-05-01 15:34:48.000000 syncqb-1.0.6/src/syncqb.egg-info/top_level.txt
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-01 15:34:48.937323 syncqb-1.0.6/tests/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     4217 2023-05-01 15:18:47.000000 syncqb-1.0.6/tests/test.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-05 15:56:00.054428 syncqb-1.0.7/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1073 2022-09-12 17:13:14.000000 syncqb-1.0.7/LICENSE
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-05-05 15:56:00.054428 syncqb-1.0.7/PKG-INFO
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     8642 2023-04-05 20:53:17.000000 syncqb-1.0.7/README.md
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      749 2023-05-05 15:49:28.000000 syncqb-1.0.7/pyproject.toml
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       38 2023-05-05 15:56:00.054428 syncqb-1.0.7/setup.cfg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       82 2023-04-06 20:44:31.000000 syncqb-1.0.7/setup.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-05 15:56:00.043595 syncqb-1.0.7/src/
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-05 15:56:00.043595 syncqb-1.0.7/src/syncqb/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2022-09-12 14:58:01.000000 syncqb-1.0.7/src/syncqb/__init__.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2023-03-29 20:36:22.000000 syncqb-1.0.7/src/syncqb/__init__.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    17107 2023-05-05 15:50:30.000000 syncqb-1.0.7/src/syncqb/json_quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    13019 2023-05-05 15:40:29.000000 syncqb-1.0.7/src/syncqb/json_quickbase.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     2193 2023-05-05 15:50:43.000000 syncqb-1.0.7/src/syncqb/qb_client.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1665 2023-04-13 17:14:40.000000 syncqb-1.0.7/src/syncqb/qb_client.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1310 2023-04-07 16:31:57.000000 syncqb-1.0.7/src/syncqb/qb_errors.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1046 2023-04-07 14:18:00.000000 syncqb-1.0.7/src/syncqb/qb_errors.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     3274 2023-05-05 15:51:25.000000 syncqb-1.0.7/src/syncqb/quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      588 2023-04-07 14:18:23.000000 syncqb-1.0.7/src/syncqb/quickbase.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     4205 2023-05-04 21:04:24.000000 syncqb-1.0.7/src/syncqb/test.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    25524 2023-05-05 15:50:56.000000 syncqb-1.0.7/src/syncqb/xml_quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     8783 2023-04-07 14:18:50.000000 syncqb-1.0.7/src/syncqb/xml_quickbase.pyi
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-05 15:56:00.043595 syncqb-1.0.7/src/syncqb.egg-info/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-05-05 15:56:00.000000 syncqb-1.0.7/src/syncqb.egg-info/PKG-INFO
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      576 2023-05-05 15:56:00.000000 syncqb-1.0.7/src/syncqb.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        1 2023-05-05 15:56:00.000000 syncqb-1.0.7/src/syncqb.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       59 2023-05-05 15:56:00.000000 syncqb-1.0.7/src/syncqb.egg-info/entry_points.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       44 2023-05-05 15:56:00.000000 syncqb-1.0.7/src/syncqb.egg-info/requires.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        7 2023-05-05 15:56:00.000000 syncqb-1.0.7/src/syncqb.egg-info/top_level.txt
```

### Comparing `syncqb-1.0.6/LICENSE` & `syncqb-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.6/PKG-INFO` & `syncqb-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncqb
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python SDK for quickbase
 Author-email: Jacob Gearhardt <jacob@synctivate.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `syncqb-1.0.6/README.md` & `syncqb-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.6/pyproject.toml` & `syncqb-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0",'requests>=2.25.1','lxml>=4.6.3','chardet>=3.0.4']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "syncqb"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Jacob Gearhardt", email="jacob@synctivate.com" },
 ]
 description = "A Python SDK for quickbase"
 readme = "README.md"
 license = { file="LICENSE" }
 dependencies = [
```

### Comparing `syncqb-1.0.6/src/syncqb/json_quickbase.py` & `syncqb-1.0.7/src/syncqb/json_quickbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,40 +20,56 @@
             raise QBAuthError("In order to use this SDK, you must provide a Quickbase user token.")
         
         self.default = default
 
     # ---------------------------------------- formatting functions ----------------------------------------
     def nest(self, data_list):
         for index, data in enumerate(data_list):
-            data_list[index] = {key: {'value': value} for key, value in data.items()}
+            data_list[index] = self.nest_record(data)
 
         return data_list
 
     def denest(self, data_list):
         for index, data in enumerate(data_list):
-            data_list[index] = {key: value['value'] for key, value in data.items()}
+            data_list[index] = self.denest_record(data)
 
         return data_list
     
     def replace_empty_values(self, data_list, default_value):
         for index, data in enumerate(data_list):
-            data_list[index] = {key: default_value if value is None else value for key, value in data.items()}
+            data_list[index] = self.replace_empty_values_record(data, default_value)
 
         return data_list
 
     def none_to_0(self, data_list):
         return self.replace_empty_values(data_list, 0)
 
     def round_ints(self, data_list):
         for index, data in enumerate(data_list):
-            for key, value in data.items():
-                if isinstance(value, float) and value.is_integer():
-                    data_list[index][key] = int(value)
+            data_list[index] = self.round_ints_record(data)
 
         return data_list
+    
+    def nest_record(self, data):
+        return {key: {'value': value} for key, value in data.items()}
+    
+    def denest_record(self, data):
+        return {key: value['value'] for key, value in data.items()}
+    
+    def replace_empty_values_record(self, data, default_value):
+        return {key: default_value if value is None else value for key, value in data.items()}
+    
+    def none_to_0_record(self, data):
+        return self.replace_empty_values_record(data, 0)
+    
+    def round_ints_record(self, data):
+        for key, value in data.items():
+            if isinstance(value, float) and value.is_integer():
+                data[key] = int(value)
+        return data
     # ---------------------------------------- info gathering functions ----------------------------------------
     def _get_sort_list(self, fids, ascending):
         if ascending:
             order = 'ASC'
         else:
             order = 'DESC'
 
@@ -141,20 +157,20 @@
             response = self._get_data(body, skip, num, require_all)
         else:
             raise ValueError('Must provide either a query or a qid')
 
         if default == None:
             default = self.default
         
-
-        data = self.denest(response)
-        data = self.replace_empty_values(data, default)
-
-        if round_ints:
-            data = self.round_ints(data)
+        for index, data in enumerate(response):
+            data = self.denest_record(data)
+            data = self.replace_empty_values_record(data, default)
+            if round_ints:
+                data = self.round_ints_record(data)
+            response[index] = data
 
         return data
 
     def _run_report(self, qid, database=None, skip=None, top=None):
         params = {
             'tableId': database or self.database,
             'skip': skip,
```

### Comparing `syncqb-1.0.6/src/syncqb/json_quickbase.pyi` & `syncqb-1.0.7/src/syncqb/json_quickbase.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,56 @@
     def round_ints(self, data_list: list[dict[str, Any]]) ->  list[dict[str, Any]]: 
         """
         Takes a list of dictionaries and rounds all float values that are actually integers.
         :param data_list: (list of dict) your list of record data
         :return: (list of dict) your list of record data
         """
         ...
+
+    
+    def nest_record(self, data: dict[str, Any])-> dict[str, Any]:
+        """
+        Takes a single record from a returned data list and nests the values in a dictionary with a 'value' key.
+        :param data: (dict) single record data denested
+        :return: (dict) your data record
+        """
+        ...
+    
+    def denest_record(self, data: dict[str, Any])-> dict[str, Any]:
+        """
+        Takes a single record from a returned data list and removes the 'value' key from the values.
+        :param data: (dict) single record data nested
+        :return: (dict) your data record
+        """
+        ...
+    
+    def replace_empty_values_record(self, data: dict[str, Any], default_value: Any)-> dict[str, Any]:
+        """
+        Takes a single record from a returned data list and replaces None values with a given default value.
+        :param data: (dict) single record data denested
+        :param default_value: (Any) default value to replace
+        :return: (dict) your data record
+        """
+        ...
+    
+    def none_to_0_record(self, data: dict[str, Any])-> dict[str, Any]:
+        """
+        DEPRECATED: Use replace_empty_values_record instead
+        :param data: (dict) single record data denested
+        :return: (dict) your data record
+        """
+        ...
+    
+    def round_ints_record(self, data: dict[str, Any])-> dict[str, Any]:
+        """
+        Takes a single record from a returned data list and rounds all float values that are actually integers.
+        :param data: (dict) single record data denested
+        :return: (dict) your data record
+        """
+        ...
     def get_schema(self, database: str | None = None, include_permissions: bool = False) -> list[dict[str, Any]]: 
         """
         Get the schema of a Quickbase table.
         :param database: (str or None) Quickbase Table ID (default None, uses self.database)
         :param include_permissions: (bool) Whether to include permissions in the schema (default False)
         :return: (list of dict) your list of record data
         """
```

### Comparing `syncqb-1.0.6/src/syncqb/qb_client.py` & `syncqb-1.0.7/src/syncqb/qb_client.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.6/src/syncqb/qb_client.pyi` & `syncqb-1.0.7/src/syncqb/qb_client.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.6/src/syncqb/qb_errors.py` & `syncqb-1.0.7/src/syncqb/qb_errors.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.6/src/syncqb/qb_errors.pyi` & `syncqb-1.0.7/src/syncqb/qb_errors.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.6/src/syncqb/quickbase.py` & `syncqb-1.0.7/src/syncqb/quickbase.py`

 * *Files 13% similar despite different names*

```diff
@@ -61,15 +61,23 @@
         
     def _request(self, url, action, headers, data=None, params=None, json=False):
         tries = 0
 
         while tries < 10:
             try:
                 return self._make_request(url, action, headers, params=params, data=data, json=json)
-            except requests.exceptions.Timeout or QBResponseError as e:
+            except requests.exceptions.Timeout as e:
                 tries += 1
-                if type(e) == QBResponseError:
+                time.sleep(1)
+                pass
+            except QBResponseError as e:
+                if e.response.status_code == 429:
+                    tries += 1
+                    time.sleep(5)
+                    pass
+                if e.response.status_code == 504:
+                    tries += 1
                     time.sleep(30)
+                    pass
                 else:
-                    time.sleep(1)
-                pass
+                    raise e from e
         raise QBConnectionError('Connection Error: Timeout')
```

### Comparing `syncqb-1.0.6/src/syncqb/quickbase.pyi` & `syncqb-1.0.7/src/syncqb/quickbase.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.6/src/syncqb/xml_quickbase.py` & `syncqb-1.0.7/src/syncqb/xml_quickbase.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.6/src/syncqb/xml_quickbase.pyi` & `syncqb-1.0.7/src/syncqb/xml_quickbase.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.6/src/syncqb.egg-info/PKG-INFO` & `syncqb-1.0.7/src/syncqb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncqb
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python SDK for quickbase
 Author-email: Jacob Gearhardt <jacob@synctivate.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `syncqb-1.0.6/src/syncqb.egg-info/SOURCES.txt` & `syncqb-1.0.7/src/syncqb.egg-info/SOURCES.txt`

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
+src/syncqb/test.py
 src/syncqb/xml_quickbase.py
 src/syncqb/xml_quickbase.pyi
 src/syncqb.egg-info/PKG-INFO
 src/syncqb.egg-info/SOURCES.txt
 src/syncqb.egg-info/dependency_links.txt
 src/syncqb.egg-info/entry_points.txt
 src/syncqb.egg-info/requires.txt
-src/syncqb.egg-info/top_level.txt
-tests/test.py
+src/syncqb.egg-info/top_level.txt
```

### Comparing `syncqb-1.0.6/tests/test.py` & `syncqb-1.0.7/src/syncqb/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -238,28 +238,28 @@
     # )
     xml_res = 'N/A'
     json_res = client2.do_query(
         query=main_asset_query,
         database=database,
         columns=columns,
         # high_volume=True,
-        # require_all=True,
+        require_all=True,
     )
     # json_res = client2.do_query(
     #     query='{3.EX.128}',
     #     # qid=10,
     #     columns=[3, 6, 9], 
     #     database='bnsucj684',
     # )
     # json_res = 'N/A'
 
     # print('xml_res:', xml_res)
     # for record in json_res:
     #     print(record)
-    print('json_res:', json_res)
+    print('json_res:')
     
 
 
 
 
 if __name__ == '__main__':
     main()
```

