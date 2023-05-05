# Comparing `tmp/NikeCA-0.1.92.tar.gz` & `tmp/NikeCA-0.1.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.92.tar", last modified: Fri May  5 04:25:42 2023, max compression
+gzip compressed data, was "NikeCA-0.1.93.tar", last modified: Fri May  5 21:40:24 2023, max compression
```

## Comparing `NikeCA-0.1.92.tar` & `NikeCA-0.1.93.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 04:25:42.737021 NikeCA-0.1.92/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.92/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-05 04:25:42.736486 NikeCA-0.1.92/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.92/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-05 04:25:42.737153 NikeCA-0.1.92/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2503 2023-05-05 04:25:37.000000 NikeCA-0.1.92/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 04:25:42.728345 NikeCA-0.1.92/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 04:25:42.729588 NikeCA-0.1.92/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     3966 2023-05-04 22:56:58.000000 NikeCA-0.1.92/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 04:25:42.730812 NikeCA-0.1.92/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-03 02:40:56.000000 NikeCA-0.1.92/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.92/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 04:25:42.732991 NikeCA-0.1.92/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.1.92/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     6080 2023-05-05 04:19:50.000000 NikeCA-0.1.92/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.1.92/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.92/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 04:25:42.735771 NikeCA-0.1.92/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-05 04:25:42.000000 NikeCA-0.1.92/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-05 04:25:42.000000 NikeCA-0.1.92/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-05 04:25:42.000000 NikeCA-0.1.92/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-05 04:25:42.000000 NikeCA-0.1.92/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-05 04:25:42.000000 NikeCA-0.1.92/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      415 2023-05-03 02:40:56.000000 NikeCA-0.1.92/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.1.92/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    23789 2023-05-05 04:24:30.000000 NikeCA-0.1.92/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.1.92/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.1.92/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.1.92/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.1.92/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-05-04 17:11:39.000000 NikeCA-0.1.92/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-04 17:07:22.000000 NikeCA-0.1.92/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-05-03 02:40:56.000000 NikeCA-0.1.92/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.1.92/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 21:40:24.526112 NikeCA-0.1.93/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.93/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-05 21:40:24.525748 NikeCA-0.1.93/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.93/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-05 21:40:24.526225 NikeCA-0.1.93/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2503 2023-05-05 21:40:02.000000 NikeCA-0.1.93/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 21:40:24.519731 NikeCA-0.1.93/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 21:40:24.520902 NikeCA-0.1.93/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3966 2023-05-04 22:56:58.000000 NikeCA-0.1.93/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 21:40:24.521926 NikeCA-0.1.93/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-03 02:40:56.000000 NikeCA-0.1.93/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.93/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 21:40:24.523423 NikeCA-0.1.93/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.1.93/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6090 2023-05-05 21:36:15.000000 NikeCA-0.1.93/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.1.93/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.93/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 21:40:24.525193 NikeCA-0.1.93/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-05 21:40:24.000000 NikeCA-0.1.93/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-05 21:40:24.000000 NikeCA-0.1.93/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-05 21:40:24.000000 NikeCA-0.1.93/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-05 21:40:24.000000 NikeCA-0.1.93/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-05 21:40:24.000000 NikeCA-0.1.93/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      415 2023-05-03 02:40:56.000000 NikeCA-0.1.93/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.1.93/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    23789 2023-05-05 04:24:30.000000 NikeCA-0.1.93/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.1.93/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.1.93/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.1.93/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.1.93/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-05-04 17:11:39.000000 NikeCA-0.1.93/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-04 17:07:22.000000 NikeCA-0.1.93/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-05-03 02:40:56.000000 NikeCA-0.1.93/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.1.93/src/__init__.py
```

### Comparing `NikeCA-0.1.92/LICENSE` & `NikeCA-0.1.93/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.92/PKG-INFO` & `NikeCA-0.1.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.92
+Version: 0.1.93
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.92/README.md` & `NikeCA-0.1.93/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.92/setup.py` & `NikeCA-0.1.93/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.92',
+	version='0.1.93',
 	description='Standardize and Automate processes',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"Dashboards/__init__",
```

### Comparing `NikeCA-0.1.92/src/Dashboards/Dashboards.py` & `NikeCA-0.1.93/src/Dashboards/Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.92/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.1.93/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.92/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.1.93/src/Dashboards/Telemetry/ProductUsage.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.92/src/Dashboards/Telemetry/Telemetry.py` & `NikeCA-0.1.93/src/Dashboards/Telemetry/Telemetry.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                 */
                 SELECT 
                     {b}
                     , PRODUCT_NAME
                     , SUM(DAILY_USAGE) AS TOTAL_USAGE
                 FROM (
 
-                {self.get_base_query(start_date=start_date, end_date=end_date)}
+                {self.telemetry_get_base_query(start_date=start_date, end_date=end_date)}
 
                 )
 
                 GROUP BY 
                     {b}
                     , PRODUCT_NAME
```

### Comparing `NikeCA-0.1.92/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.93/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.92
+Version: 0.1.93
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.92/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.1.93/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.92/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.93/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.92/src/NikeQA.py` & `NikeCA-0.1.93/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.92/src/NikeSF.py` & `NikeCA-0.1.93/src/NikeSF.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.92/src/_BuildSearchQuery.py` & `NikeCA-0.1.93/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.92/src/_GitHub.py` & `NikeCA-0.1.93/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.92/src/_QA.py` & `NikeCA-0.1.93/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.92/src/_SearchFiles.py` & `NikeCA-0.1.93/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.92/src/_SnowflakeData.py` & `NikeCA-0.1.93/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.92/src/_SnowflakeDependencies.py` & `NikeCA-0.1.93/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.92/src/_SnowflakePull.py` & `NikeCA-0.1.93/src/_SnowflakePull.py`

 * *Files identical despite different names*

