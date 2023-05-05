# Comparing `tmp/yetl-framework-1.0.1.tar.gz` & `tmp/yetl-framework-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.0.1.tar", last modified: Fri May  5 08:06:18 2023, max compression
+gzip compressed data, was "yetl-framework-1.0.2.tar", last modified: Fri May  5 17:09:03 2023, max compression
```

## Comparing `yetl-framework-1.0.1.tar` & `yetl-framework-1.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-05 08:06:18.139489 yetl-framework-1.0.1/
--rw-r--r--   0 vsts      (1001) docker     (123)     5770 2023-05-05 08:06:18.139489 yetl-framework-1.0.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     5273 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-05 08:06:18.139489 yetl-framework-1.0.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1043 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-05 08:06:18.131489 yetl-framework-1.0.1/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      455 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3220 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1994 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      158 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      305 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7311 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4717 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-05 08:06:18.135489 yetl-framework-1.0.1/yetl/dataset/
--rw-r--r--   0 vsts      (1001) docker     (123)      217 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1268 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/dataset/_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3425 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/dataset/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4032 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/dataset/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5274 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/dataset/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/dataset/_write.py
--rw-r--r--   0 vsts      (1001) docker     (123)      198 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/dataset/dataset_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7666 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-05 08:06:18.135489 yetl-framework-1.0.1/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-05 08:06:18.139489 yetl-framework-1.0.1/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5770 2023-05-05 08:06:18.000000 yetl-framework-1.0.1/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      734 2023-05-05 08:06:18.000000 yetl-framework-1.0.1/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-05 08:06:18.000000 yetl-framework-1.0.1/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-05 08:06:18.000000 yetl-framework-1.0.1/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-05 08:06:18.000000 yetl-framework-1.0.1/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-05 08:06:18.000000 yetl-framework-1.0.1/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-05 17:09:03.087733 yetl-framework-1.0.2/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5770 2023-05-05 17:09:03.087733 yetl-framework-1.0.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     5273 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-05 17:09:03.087733 yetl-framework-1.0.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1043 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-05 17:09:03.087733 yetl-framework-1.0.2/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      455 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3220 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1994 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      158 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      305 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7313 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4717 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-05 17:09:03.087733 yetl-framework-1.0.2/yetl/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (123)      217 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1268 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/dataset/_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3425 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/dataset/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4032 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/dataset/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5274 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/dataset/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/dataset/_write.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      198 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/dataset/dataset_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7666 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-05 17:09:03.087733 yetl-framework-1.0.2/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-05 17:08:07.000000 yetl-framework-1.0.2/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-05 17:09:03.087733 yetl-framework-1.0.2/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5770 2023-05-05 17:09:03.000000 yetl-framework-1.0.2/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      734 2023-05-05 17:09:03.000000 yetl-framework-1.0.2/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-05 17:09:03.000000 yetl-framework-1.0.2/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-05 17:09:03.000000 yetl-framework-1.0.2/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-05 17:09:03.000000 yetl-framework-1.0.2/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-05 17:09:03.000000 yetl-framework-1.0.2/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.0.1/PKG-INFO` & `yetl-framework-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.0.1
+Version: 1.0.2
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.0.1/README.md` & `yetl-framework-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.1/setup.py` & `yetl-framework-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.0.1",
+    version="1.0.2",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.0.1/yetl/_config.py` & `yetl-framework-1.0.2/yetl/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.1/yetl/_decorators.py` & `yetl-framework-1.0.2/yetl/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.1/yetl/_logging_config.py` & `yetl-framework-1.0.2/yetl/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.1/yetl/_project.py` & `yetl-framework-1.0.2/yetl/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.1/yetl/_spark_context.py` & `yetl-framework-1.0.2/yetl/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.1/yetl/_tables.py` & `yetl-framework-1.0.2/yetl/_tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,18 +149,18 @@
             for p, v in properties.items():
                 if (
                     isinstance(table.custom_properties, dict)
                     and table.custom_properties.get(p) == v
                 ):
                     return True
                 else:
-                    index = Tables.get_index(table.stage, table.database, table.name)
+                    index = Tables.get_index(table.stage, table.database, table.table)
                     if index in matches:
                         matches.remove(
-                            Tables.get_index(table.stage, table.database, table.name)
+                            Tables.get_index(table.stage, table.database, table.table)
                         )
                     return False
 
         tables_index = dict(self.tables_index)
         if kwargs:
             tables_index = {
                 k: v
```

### Comparing `yetl-framework-1.0.1/yetl/_timeslice.py` & `yetl-framework-1.0.2/yetl/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.1/yetl/_utils.py` & `yetl-framework-1.0.2/yetl/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.1/yetl/dataset/_dataset.py` & `yetl-framework-1.0.2/yetl/dataset/_dataset.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.1/yetl/dataset/_deltalake.py` & `yetl-framework-1.0.2/yetl/dataset/_deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.1/yetl/dataset/_factory.py` & `yetl-framework-1.0.2/yetl/dataset/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.1/yetl/dataset/_read.py` & `yetl-framework-1.0.2/yetl/dataset/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.1/yetl/deltalake.py` & `yetl-framework-1.0.2/yetl/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.1/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.0.2/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.1/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.0.2/yetl_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.0.1
+Version: 1.0.2
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.0.1/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.0.2/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

