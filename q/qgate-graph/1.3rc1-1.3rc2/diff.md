# Comparing `tmp/qgate_graph-1.3rc1.tar.gz` & `tmp/qgate_graph-1.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgate_graph-1.3rc1.tar", last modified: Mon May  1 17:51:51 2023, max compression
+gzip compressed data, was "qgate_graph-1.3rc2.tar", last modified: Thu May  4 20:55:11 2023, max compression
```

## Comparing `qgate_graph-1.3rc1.tar` & `qgate_graph-1.3rc2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 17:51:51.075504 qgate_graph-1.3rc1/
--rw-rw-rw-   0        0        0      135 2023-04-27 20:50:17.000000 qgate_graph-1.3rc1/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-01 17:51:50.889433 qgate_graph-1.3rc1/.idea/
--rw-rw-rw-   0        0        0       50 2023-04-27 15:39:54.000000 qgate_graph-1.3rc1/.idea/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-01 17:51:50.907517 qgate_graph-1.3rc1/.idea/inspectionProfiles/
--rw-rw-rw-   0        0        0    12870 2023-04-27 16:54:16.000000 qgate_graph-1.3rc1/.idea/inspectionProfiles/Project_Default.xml
--rw-rw-rw-   0        0        0      174 2023-04-27 16:54:16.000000 qgate_graph-1.3rc1/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0        0        0      321 2023-04-27 16:54:16.000000 qgate_graph-1.3rc1/.idea/misc.xml
--rw-rw-rw-   0        0        0      281 2023-04-27 16:54:16.000000 qgate_graph-1.3rc1/.idea/modules.xml
--rw-rw-rw-   0        0        0      361 2023-04-27 16:54:16.000000 qgate_graph-1.3rc1/.idea/qgate-graph.iml
--rw-rw-rw-   0        0        0      185 2023-04-27 20:07:09.000000 qgate_graph-1.3rc1/.idea/vcs.xml
--rw-rw-rw-   0        0        0     1171 2023-05-01 17:51:51.072502 qgate_graph-1.3rc1/PKG-INFO
--rw-rw-rw-   0        0        0      792 2023-05-01 17:49:29.000000 qgate_graph-1.3rc1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 17:51:50.923160 qgate_graph-1.3rc1/assets/
--rw-rw-rw-   0        0        0   117721 2023-04-29 10:46:59.000000 qgate_graph-1.3rc1/assets/NoSQL_bdp_nonprod-2023-04-22_17-08-34-bulk-10000x50.png
--rw-rw-rw-   0        0        0     1672 2023-04-29 14:30:45.000000 qgate_graph-1.3rc1/dependencies.py
--rw-rw-rw-   0        0        0       29 2023-04-29 13:39:22.000000 qgate_graph-1.3rc1/dev-requirements.txt
--rw-rw-rw-   0        0        0      795 2023-05-01 17:41:15.000000 qgate_graph-1.3rc1/main.py
--rwxrwxrwx   0        0        0      171 2023-05-01 17:49:29.000000 qgate_graph-1.3rc1/publish.bat
-drwxrwxrwx   0        0        0        0 2023-05-01 17:51:50.989951 qgate_graph-1.3rc1/qgate_graph/
--rw-rw-rw-   0        0        0       15 2023-04-27 20:40:11.000000 qgate_graph-1.3rc1/qgate_graph/.gitignore
--rw-rw-rw-   0        0        0       40 2023-04-29 09:53:53.000000 qgate_graph-1.3rc1/qgate_graph/__init__.py
--rw-rw-rw-   0        0        0     1057 2023-04-30 11:34:41.000000 qgate_graph-1.3rc1/qgate_graph/file_format.py
--rw-rw-rw-   0        0        0     2378 2023-05-01 17:36:42.000000 qgate_graph-1.3rc1/qgate_graph/graph_base.py
--rw-rw-rw-   0        0        0     7360 2023-05-01 17:36:42.000000 qgate_graph-1.3rc1/qgate_graph/graph_executor.py
--rw-rw-rw-   0        0        0     7150 2023-05-01 17:36:42.000000 qgate_graph-1.3rc1/qgate_graph/graph_performance.py
--rw-rw-rw-   0        0        0      216 2023-05-01 17:51:08.000000 qgate_graph-1.3rc1/qgate_graph/version.py
-drwxrwxrwx   0        0        0        0 2023-05-01 17:51:51.059489 qgate_graph-1.3rc1/qgate_graph.egg-info/
--rw-rw-rw-   0        0        0     1171 2023-05-01 17:51:49.000000 qgate_graph-1.3rc1/qgate_graph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      704 2023-05-01 17:51:50.000000 qgate_graph-1.3rc1/qgate_graph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 17:51:49.000000 qgate_graph-1.3rc1/qgate_graph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-01 17:51:49.000000 qgate_graph-1.3rc1/qgate_graph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-01 17:51:49.000000 qgate_graph-1.3rc1/qgate_graph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       19 2023-04-29 13:39:54.000000 qgate_graph-1.3rc1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 17:51:51.076490 qgate_graph-1.3rc1/setup.cfg
--rw-rw-rw-   0        0        0     1257 2023-04-29 14:36:28.000000 qgate_graph-1.3rc1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:55:11.173330 qgate_graph-1.3rc2/
+-rw-rw-rw-   0        0        0      135 2023-04-27 20:50:17.000000 qgate_graph-1.3rc2/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-04 20:55:10.901148 qgate_graph-1.3rc2/.idea/
+-rw-rw-rw-   0        0        0       50 2023-04-27 15:39:54.000000 qgate_graph-1.3rc2/.idea/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-04 20:55:10.931403 qgate_graph-1.3rc2/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0    12870 2023-04-27 16:54:16.000000 qgate_graph-1.3rc2/.idea/inspectionProfiles/Project_Default.xml
+-rw-rw-rw-   0        0        0      174 2023-04-27 16:54:16.000000 qgate_graph-1.3rc2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      321 2023-04-27 16:54:16.000000 qgate_graph-1.3rc2/.idea/misc.xml
+-rw-rw-rw-   0        0        0      281 2023-04-27 16:54:16.000000 qgate_graph-1.3rc2/.idea/modules.xml
+-rw-rw-rw-   0        0        0      361 2023-04-27 16:54:16.000000 qgate_graph-1.3rc2/.idea/qgate-graph.iml
+-rw-rw-rw-   0        0        0      185 2023-04-27 20:07:09.000000 qgate_graph-1.3rc2/.idea/vcs.xml
+-rw-rw-rw-   0        0        0     1169 2023-05-04 20:55:11.169223 qgate_graph-1.3rc2/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2023-05-01 18:07:42.000000 qgate_graph-1.3rc2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 20:55:10.955666 qgate_graph-1.3rc2/assets/
+-rw-rw-rw-   0        0        0   117721 2023-04-29 10:46:59.000000 qgate_graph-1.3rc2/assets/NoSQL_bdp_nonprod-2023-04-22_17-08-34-bulk-10000x50.png
+-rw-rw-rw-   0        0        0     1672 2023-04-29 14:30:45.000000 qgate_graph-1.3rc2/dependencies.py
+-rw-rw-rw-   0        0        0       29 2023-04-29 13:39:22.000000 qgate_graph-1.3rc2/dev-requirements.txt
+-rw-rw-rw-   0        0        0      795 2023-05-01 17:41:15.000000 qgate_graph-1.3rc2/main.py
+-rwxrwxrwx   0        0        0      171 2023-05-01 17:49:29.000000 qgate_graph-1.3rc2/publish.bat
+drwxrwxrwx   0        0        0        0 2023-05-04 20:55:11.066332 qgate_graph-1.3rc2/qgate_graph/
+-rw-rw-rw-   0        0        0       15 2023-04-27 20:40:11.000000 qgate_graph-1.3rc2/qgate_graph/.gitignore
+-rw-rw-rw-   0        0        0       40 2023-04-29 09:53:53.000000 qgate_graph-1.3rc2/qgate_graph/__init__.py
+-rw-rw-rw-   0        0        0     1057 2023-04-30 11:34:41.000000 qgate_graph-1.3rc2/qgate_graph/file_format.py
+-rw-rw-rw-   0        0        0     2378 2023-05-01 17:36:42.000000 qgate_graph-1.3rc2/qgate_graph/graph_base.py
+-rw-rw-rw-   0        0        0     7378 2023-05-04 20:53:30.000000 qgate_graph-1.3rc2/qgate_graph/graph_executor.py
+-rw-rw-rw-   0        0        0     7150 2023-05-01 17:36:42.000000 qgate_graph-1.3rc2/qgate_graph/graph_performance.py
+-rw-rw-rw-   0        0        0      216 2023-05-04 20:54:48.000000 qgate_graph-1.3rc2/qgate_graph/version.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:55:11.152926 qgate_graph-1.3rc2/qgate_graph.egg-info/
+-rw-rw-rw-   0        0        0     1169 2023-05-04 20:55:09.000000 qgate_graph-1.3rc2/qgate_graph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      704 2023-05-04 20:55:10.000000 qgate_graph-1.3rc2/qgate_graph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 20:55:09.000000 qgate_graph-1.3rc2/qgate_graph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-04 20:55:09.000000 qgate_graph-1.3rc2/qgate_graph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-04 20:55:09.000000 qgate_graph-1.3rc2/qgate_graph.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       19 2023-04-29 13:39:54.000000 qgate_graph-1.3rc2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 20:55:11.174323 qgate_graph-1.3rc2/setup.cfg
+-rw-rw-rw-   0        0        0     1257 2023-04-29 14:36:28.000000 qgate_graph-1.3rc2/setup.py
```

### Comparing `qgate_graph-1.3rc1/.idea/inspectionProfiles/Project_Default.xml` & `qgate_graph-1.3rc2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.3rc1/PKG-INFO` & `qgate_graph-1.3rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate_graph
-Version: 1.3rc1
+Version: 1.3rc2
 Summary: Generate graphs based on outputs from Quality Gate
 Home-page: https://github.com/george0st/qgate-graph/
 Download-URL: https://pypi.org/project/qgate_graph/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: Quality,QualityGate,Graph
@@ -29,13 +29,12 @@
     # generate performance/throughput graphs
     graph=GraphPerformance()
     graph.generate_from_dir()
     
     # generate excutors in time graphs
     graph=grp.GraphExecutor()
     graph.generate_from_dir()
-
 ```
 
 # Outputs
 ![graph](./assets/NoSQL_bdp_nonprod-2023-04-22_17-08-34-bulk-10000x50.png)
```

### Comparing `qgate_graph-1.3rc1/README.md` & `qgate_graph-1.3rc2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,13 +17,12 @@
     # generate performance/throughput graphs
     graph=GraphPerformance()
     graph.generate_from_dir()
     
     # generate excutors in time graphs
     graph=grp.GraphExecutor()
     graph.generate_from_dir()
-
 ```
 
 # Outputs
 ![graph](./assets/NoSQL_bdp_nonprod-2023-04-22_17-08-34-bulk-10000x50.png)
```

### Comparing `qgate_graph-1.3rc1/assets/NoSQL_bdp_nonprod-2023-04-22_17-08-34-bulk-10000x50.png` & `qgate_graph-1.3rc2/assets/NoSQL_bdp_nonprod-2023-04-22_17-08-34-bulk-10000x50.png`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.3rc1/dependencies.py` & `qgate_graph-1.3rc2/dependencies.py`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.3rc1/main.py` & `qgate_graph-1.3rc2/main.py`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.3rc1/qgate_graph/file_format.py` & `qgate_graph-1.3rc2/qgate_graph/file_format.py`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.3rc1/qgate_graph/graph_base.py` & `qgate_graph-1.3rc2/qgate_graph/graph_base.py`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.3rc1/qgate_graph/graph_executor.py` & `qgate_graph-1.3rc2/qgate_graph/graph_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,16 @@
                     if executor:
                         plan=f"{input_dict[const.FileFormat.PRF_CORE_PLAN_EXECUTOR][0]},{input_dict[const.FileFormat.PRF_CORE_PLAN_EXECUTOR][1]}"
                         executors[plan]=executor
 
                         if input_dict.get(const.FileFormat.PRF_CORE_TIME_END):
                             end_date=input_dict[const.FileFormat.PRF_CORE_TIME_END]
 
-                        file_name=f"{file_name}-plan-{plan}"
-                        self._show_graph(start_date, executors, end_date, title, file_name, output_dir)
+                        #file_name=f"{file_name}-plan-{plan}"
+                        self._show_graph(start_date, executors, end_date, title, f"{file_name}-plan-{plan}", output_dir)
                         executors.clear()
                         executor.clear()
                 elif input_dict[const.FileFormat.PRF_TYPE] == const.FileFormat.PRF_DETAIL_TYPE:
                     # detail
                     executor.append([
                         input_dict[const.FileFormat.PRF_DETAIL_TIME_INIT],
                         input_dict[const.FileFormat.PRF_DETAIL_TIME_START],
```

### Comparing `qgate_graph-1.3rc1/qgate_graph/graph_performance.py` & `qgate_graph-1.3rc2/qgate_graph/graph_performance.py`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.3rc1/qgate_graph.egg-info/PKG-INFO` & `qgate_graph-1.3rc2/qgate_graph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate-graph
-Version: 1.3rc1
+Version: 1.3rc2
 Summary: Generate graphs based on outputs from Quality Gate
 Home-page: https://github.com/george0st/qgate-graph/
 Download-URL: https://pypi.org/project/qgate_graph/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: Quality,QualityGate,Graph
@@ -29,13 +29,12 @@
     # generate performance/throughput graphs
     graph=GraphPerformance()
     graph.generate_from_dir()
     
     # generate excutors in time graphs
     graph=grp.GraphExecutor()
     graph.generate_from_dir()
-
 ```
 
 # Outputs
 ![graph](./assets/NoSQL_bdp_nonprod-2023-04-22_17-08-34-bulk-10000x50.png)
```

### Comparing `qgate_graph-1.3rc1/qgate_graph.egg-info/SOURCES.txt` & `qgate_graph-1.3rc2/qgate_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.3rc1/setup.py` & `qgate_graph-1.3rc2/setup.py`

 * *Files identical despite different names*

