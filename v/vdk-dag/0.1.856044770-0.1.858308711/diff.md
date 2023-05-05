# Comparing `tmp/vdk-dag-0.1.856044770.tar.gz` & `tmp/vdk-dag-0.1.858308711.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-dag-0.1.856044770.tar", last modified: Wed May  3 17:36:56 2023, max compression
+gzip compressed data, was "vdk-dag-0.1.858308711.tar", last modified: Fri May  5 11:30:46 2023, max compression
```

## Comparing `vdk-dag-0.1.856044770.tar` & `vdk-dag-0.1.858308711.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:36:56.338122 vdk-dag-0.1.856044770/
--rw-r--r--   0 root         (0) root         (0)     8339 2023-05-03 17:36:56.338122 vdk-dag-0.1.856044770/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7772 2023-05-03 17:36:43.000000 vdk-dag-0.1.856044770/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 17:36:56.338122 vdk-dag-0.1.856044770/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-03 17:36:46.000000 vdk-dag-0.1.856044770/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:36:56.334122 vdk-dag-0.1.856044770/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:36:56.334122 vdk-dag-0.1.856044770/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:36:56.334122 vdk-dag-0.1.856044770/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:36:56.334122 vdk-dag-0.1.856044770/src/vdk/plugin/dag/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:36:56.334122 vdk-dag-0.1.856044770/src/vdk/plugin/dag/api/
--rw-rw-rw-   0 root         (0) root         (0)     1375 2023-05-03 17:36:43.000000 vdk-dag-0.1.856044770/src/vdk/plugin/dag/api/dag.py
--rw-rw-rw-   0 root         (0) root         (0)     9308 2023-05-03 17:36:43.000000 vdk-dag-0.1.856044770/src/vdk/plugin/dag/cached_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     6368 2023-05-03 17:36:43.000000 vdk-dag-0.1.856044770/src/vdk/plugin/dag/dag.py
--rw-rw-rw-   0 root         (0) root         (0)     1385 2023-05-03 17:36:43.000000 vdk-dag-0.1.856044770/src/vdk/plugin/dag/dag_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     6535 2023-05-03 17:36:43.000000 vdk-dag-0.1.856044770/src/vdk/plugin/dag/dag_plugin_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      923 2023-05-03 17:36:43.000000 vdk-dag-0.1.856044770/src/vdk/plugin/dag/dag_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     7917 2023-05-03 17:36:43.000000 vdk-dag-0.1.856044770/src/vdk/plugin/dag/dag_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     2253 2023-05-03 17:36:43.000000 vdk-dag-0.1.856044770/src/vdk/plugin/dag/dags.py
--rw-rw-rw-   0 root         (0) root         (0)     9334 2023-05-03 17:36:43.000000 vdk-dag-0.1.856044770/src/vdk/plugin/dag/remote_data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-05-03 17:36:43.000000 vdk-dag-0.1.856044770/src/vdk/plugin/dag/remote_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     2579 2023-05-03 17:36:43.000000 vdk-dag-0.1.856044770/src/vdk/plugin/dag/time_based_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:36:56.338122 vdk-dag-0.1.856044770/src/vdk_dag.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8339 2023-05-03 17:36:56.000000 vdk-dag-0.1.856044770/src/vdk_dag.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-03 17:36:56.000000 vdk-dag-0.1.856044770/src/vdk_dag.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 17:36:56.000000 vdk-dag-0.1.856044770/src/vdk_dag.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-03 17:36:56.000000 vdk-dag-0.1.856044770/src/vdk_dag.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-03 17:36:56.000000 vdk-dag-0.1.856044770/src/vdk_dag.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-03 17:36:56.000000 vdk-dag-0.1.856044770/src/vdk_dag.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:36:56.338122 vdk-dag-0.1.856044770/tests/
--rw-rw-rw-   0 root         (0) root         (0)    16367 2023-05-03 17:36:43.000000 vdk-dag-0.1.856044770/tests/test_dag.py
--rw-rw-rw-   0 root         (0) root         (0)     2550 2023-05-03 17:36:43.000000 vdk-dag-0.1.856044770/tests/test_dag_object.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-03 17:36:43.000000 vdk-dag-0.1.856044770/tests/test_time_based_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2285 2023-05-03 17:36:43.000000 vdk-dag-0.1.856044770/tests/test_tracking_job_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:30:46.411283 vdk-dag-0.1.858308711/
+-rw-r--r--   0 root         (0) root         (0)     8221 2023-05-05 11:30:46.411283 vdk-dag-0.1.858308711/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7654 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 11:30:46.411283 vdk-dag-0.1.858308711/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-05 11:30:36.000000 vdk-dag-0.1.858308711/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:30:46.407283 vdk-dag-0.1.858308711/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:30:46.407283 vdk-dag-0.1.858308711/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:30:46.407283 vdk-dag-0.1.858308711/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:30:46.411283 vdk-dag-0.1.858308711/src/vdk/plugin/dag/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:30:46.411283 vdk-dag-0.1.858308711/src/vdk/plugin/dag/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/api/dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     9308 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/cached_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6078 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/dag_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6535 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/dag_plugin_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      923 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/dag_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     7917 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/dag_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2253 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/dags.py
+-rw-rw-rw-   0 root         (0) root         (0)     9334 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/remote_data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/remote_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2579 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/time_based_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:30:46.411283 vdk-dag-0.1.858308711/src/vdk_dag.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8221 2023-05-05 11:30:46.000000 vdk-dag-0.1.858308711/src/vdk_dag.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-05 11:30:46.000000 vdk-dag-0.1.858308711/src/vdk_dag.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 11:30:46.000000 vdk-dag-0.1.858308711/src/vdk_dag.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-05 11:30:46.000000 vdk-dag-0.1.858308711/src/vdk_dag.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-05 11:30:46.000000 vdk-dag-0.1.858308711/src/vdk_dag.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-05 11:30:46.000000 vdk-dag-0.1.858308711/src/vdk_dag.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:30:46.411283 vdk-dag-0.1.858308711/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    16367 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/tests/test_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2550 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/tests/test_dag_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/tests/test_time_based_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/tests/test_tracking_job_executor.py
```

### Comparing `vdk-dag-0.1.856044770/PKG-INFO` & `vdk-dag-0.1.858308711/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: vdk-dag
-Version: 0.1.856044770
+Version: 0.1.858308711
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # VDK DAGs
 
-## This plugin has been deprecated. Please use vdk-dag instead. You may install it by running `pip install vdk-dag`.
-
 Express dependencies between data jobs.
 
 A plugin for Versatile Data Kit extends its Job API with an additional feature that allows users to trigger so-called VDK DAGs.
 
 A VDK DAG is a regular Data Job that invokes other Data Jobs using Control Service Execution API.
 In this way, there's nothing different from other data jobs except for its purpose. See [Data Job types](https://github.com/vmware/versatile-data-kit/wiki/User-Guide#data-job-types) for more info.
```

### Comparing `vdk-dag-0.1.856044770/README.md` & `vdk-dag-0.1.858308711/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # VDK DAGs
 
-## This plugin has been deprecated. Please use vdk-dag instead. You may install it by running `pip install vdk-dag`.
-
 Express dependencies between data jobs.
 
 A plugin for Versatile Data Kit extends its Job API with an additional feature that allows users to trigger so-called VDK DAGs.
 
 A VDK DAG is a regular Data Job that invokes other Data Jobs using Control Service Execution API.
 In this way, there's nothing different from other data jobs except for its purpose. See [Data Job types](https://github.com/vmware/versatile-data-kit/wiki/User-Guide#data-job-types) for more info.
```

### Comparing `vdk-dag-0.1.856044770/setup.py` & `vdk-dag-0.1.858308711/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.1.856044770"
+__version__ = "0.1.858308711"
 
 setuptools.setup(
     name="vdk-dag",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Express dependecies between data jobs.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-dag-0.1.856044770/src/vdk/plugin/dag/api/dag.py` & `vdk-dag-0.1.858308711/src/vdk/plugin/dag/api/dag.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.856044770/src/vdk/plugin/dag/cached_data_job_executor.py` & `vdk-dag-0.1.858308711/src/vdk/plugin/dag/cached_data_job_executor.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.856044770/src/vdk/plugin/dag/dag.py` & `vdk-dag-0.1.858308711/src/vdk/plugin/dag/dag.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,20 +25,14 @@
     def __init__(self, team_name: str, dags_config: DagPluginConfiguration):
         """
         This module deals with all the DAG-related operations such as build and execute.
 
         :param team_name: the name of the owning team
         :param dags_config: the DAG job configuration
         """
-        log.warning(
-            "-------------------------------------------"
-            "This plugin has been deprecated. Please use vdk-dag instead. "
-            "You may install it by running `pip install vdk-dag`."
-            "-------------------------------------------"
-        )
         self._team_name = team_name
         self._topological_sorter = TopologicalSorter()
         self._delayed_starting_jobs = TimeBasedQueue(
             min_ready_time_seconds=dags_config.dags_delayed_jobs_min_delay_seconds(),
             randomize_delay_seconds=dags_config.dags_delayed_jobs_randomized_added_delay_seconds(),
         )
         self._max_concurrent_running_jobs = (
```

### Comparing `vdk-dag-0.1.856044770/src/vdk/plugin/dag/dag_plugin.py` & `vdk-dag-0.1.858308711/src/vdk/plugin/dag/dag_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.856044770/src/vdk/plugin/dag/dag_plugin_configuration.py` & `vdk-dag-0.1.858308711/src/vdk/plugin/dag/dag_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.856044770/src/vdk/plugin/dag/dag_runner.py` & `vdk-dag-0.1.858308711/src/vdk/plugin/dag/dag_runner.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.856044770/src/vdk/plugin/dag/dag_validator.py` & `vdk-dag-0.1.858308711/src/vdk/plugin/dag/dag_validator.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.856044770/src/vdk/plugin/dag/dags.py` & `vdk-dag-0.1.858308711/src/vdk/plugin/dag/dags.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.856044770/src/vdk/plugin/dag/remote_data_job.py` & `vdk-dag-0.1.858308711/src/vdk/plugin/dag/remote_data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.856044770/src/vdk/plugin/dag/remote_data_job_executor.py` & `vdk-dag-0.1.858308711/src/vdk/plugin/dag/remote_data_job_executor.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.856044770/src/vdk/plugin/dag/time_based_queue.py` & `vdk-dag-0.1.858308711/src/vdk/plugin/dag/time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.856044770/src/vdk_dag.egg-info/PKG-INFO` & `vdk-dag-0.1.858308711/src/vdk_dag.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: vdk-dag
-Version: 0.1.856044770
+Version: 0.1.858308711
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # VDK DAGs
 
-## This plugin has been deprecated. Please use vdk-dag instead. You may install it by running `pip install vdk-dag`.
-
 Express dependencies between data jobs.
 
 A plugin for Versatile Data Kit extends its Job API with an additional feature that allows users to trigger so-called VDK DAGs.
 
 A VDK DAG is a regular Data Job that invokes other Data Jobs using Control Service Execution API.
 In this way, there's nothing different from other data jobs except for its purpose. See [Data Job types](https://github.com/vmware/versatile-data-kit/wiki/User-Guide#data-job-types) for more info.
```

### Comparing `vdk-dag-0.1.856044770/src/vdk_dag.egg-info/SOURCES.txt` & `vdk-dag-0.1.858308711/src/vdk_dag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.856044770/tests/test_dag.py` & `vdk-dag-0.1.858308711/tests/test_dag.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.856044770/tests/test_dag_object.py` & `vdk-dag-0.1.858308711/tests/test_dag_object.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.856044770/tests/test_time_based_queue.py` & `vdk-dag-0.1.858308711/tests/test_time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.856044770/tests/test_tracking_job_executor.py` & `vdk-dag-0.1.858308711/tests/test_tracking_job_executor.py`

 * *Files identical despite different names*

