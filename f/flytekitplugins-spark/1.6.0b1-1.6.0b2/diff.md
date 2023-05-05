# Comparing `tmp/flytekitplugins-spark-1.6.0b1.tar.gz` & `tmp/flytekitplugins-spark-1.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-spark-1.6.0b1.tar", last modified: Wed May  3 04:48:12 2023, max compression
+gzip compressed data, was "flytekitplugins-spark-1.6.0b2.tar", last modified: Fri May  5 17:49:50 2023, max compression
```

## Comparing `flytekitplugins-spark-1.6.0b1.tar` & `flytekitplugins-spark-1.6.0b2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:12.980322 flytekitplugins-spark-1.6.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-03 04:48:12.980322 flytekitplugins-spark-1.6.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-03 04:47:44.000000 flytekitplugins-spark-1.6.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:12.976322 flytekitplugins-spark-1.6.0b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:12.980322 flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-03 04:47:44.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-05-03 04:47:44.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-03 04:47:44.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/pyspark_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-03 04:47:44.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-03 04:47:44.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/sd_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-05-03 04:47:44.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:12.980322 flytekitplugins-spark-1.6.0b1/flytekitplugins_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-03 04:48:12.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-03 04:48:12.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 04:48:12.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-03 04:48:12.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins_spark.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:12.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins_spark.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 04:48:12.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:12.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins_spark.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:12.980322 flytekitplugins-spark-1.6.0b1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-03 04:47:44.000000 flytekitplugins-spark-1.6.0b1/scripts/flytekit_install_spark3.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 04:48:12.980322 flytekitplugins-spark-1.6.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-03 04:48:03.000000 flytekitplugins-spark-1.6.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:50.162218 flytekitplugins-spark-1.6.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-05 17:49:50.162218 flytekitplugins-spark-1.6.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-05 17:49:25.000000 flytekitplugins-spark-1.6.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:50.162218 flytekitplugins-spark-1.6.0b2/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:50.162218 flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-05 17:49:25.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-05-05 17:49:25.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-05 17:49:25.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/pyspark_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-05 17:49:25.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-05 17:49:25.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/sd_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-05 17:49:25.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:50.162218 flytekitplugins-spark-1.6.0b2/flytekitplugins_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-05 17:49:50.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-05 17:49:50.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:49:50.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 17:49:50.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins_spark.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:50.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins_spark.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-05 17:49:50.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:50.000000 flytekitplugins-spark-1.6.0b2/flytekitplugins_spark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:50.162218 flytekitplugins-spark-1.6.0b2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-05 17:49:25.000000 flytekitplugins-spark-1.6.0b2/scripts/flytekit_install_spark3.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:49:50.162218 flytekitplugins-spark-1.6.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-05 17:49:40.000000 flytekitplugins-spark-1.6.0b2/setup.py
```

### Comparing `flytekitplugins-spark-1.6.0b1/PKG-INFO` & `flytekitplugins-spark-1.6.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-spark
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: Spark 3 plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-spark-1.6.0b1/README.md` & `flytekitplugins-spark-1.6.0b2/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/__init__.py` & `flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/models.py` & `flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/models.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/pyspark_transformers.py` & `flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/pyspark_transformers.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/schema.py` & `flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/sd_transformers.py` & `flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/sd_transformers.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/task.py` & `flytekitplugins-spark-1.6.0b2/flytekitplugins/spark/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
-import typing
 from dataclasses import dataclass
-from typing import Any, Callable, Dict, Optional
+from typing import Any, Callable, Dict, Optional, Union, cast
 
 from google.protobuf.json_format import MessageToDict
 from pyspark.sql import SparkSession
 
 from flytekit import FlyteContextManager, PythonFunctionTask
-from flytekit.configuration import SerializationSettings
+from flytekit.configuration import DefaultImages, SerializationSettings
 from flytekit.core.context_manager import ExecutionParameters
 from flytekit.extend import ExecutionState, TaskPlugins
+from flytekit.image_spec import ImageSpec
 
 from .models import SparkJob, SparkType
 
 
 @dataclass
 class Spark(object):
     """
@@ -44,23 +44,23 @@
 
     Args:
         databricks_conf: Databricks job configuration. Config structure can be found here. https://docs.databricks.com/dev-tools/api/2.0/jobs.html#request-structure
         databricks_token: Databricks access token. https://docs.databricks.com/dev-tools/api/latest/authentication.html.
         databricks_instance: Domain name of your deployment. Use the form <account>.cloud.databricks.com.
     """
 
-    databricks_conf: typing.Optional[Dict[str, typing.Union[str, dict]]] = None
+    databricks_conf: Optional[Dict[str, Union[str, dict]]] = None
     databricks_token: Optional[str] = None
     databricks_instance: Optional[str] = None
 
 
 # This method does not reset the SparkSession since it's a bit hard to handle multiple
 # Spark sessions in a single application as it's described in:
 # https://stackoverflow.com/questions/41491972/how-can-i-tear-down-a-sparksession-and-create-a-new-one-within-one-application.
-def new_spark_session(name: str, conf: typing.Dict[str, str] = None):
+def new_spark_session(name: str, conf: Dict[str, str] = None):
     """
     Optionally creates a new spark session and returns it.
     In cluster mode (running in hosted flyte, this will disregard the spark conf passed in)
 
     This method is safe to be used from any other method. That is one reason why, we have duplicated this code
     fragment with the pre-execute. For example in the notebook scenario we might want to call it from a separate kernel
     """
@@ -95,34 +95,51 @@
 class PysparkFunctionTask(PythonFunctionTask[Spark]):
     """
     Actual Plugin that transforms the local python code for execution within a spark context
     """
 
     _SPARK_TASK_TYPE = "spark"
 
-    def __init__(self, task_config: Spark, task_function: Callable, **kwargs):
+    def __init__(
+        self,
+        task_config: Spark,
+        task_function: Callable,
+        container_image: Optional[Union[str, ImageSpec]] = None,
+        **kwargs,
+    ):
+        self.sess: Optional[SparkSession] = None
+        self._default_executor_path: Optional[str] = None
+        self._default_applications_path: Optional[str] = None
+
+        if isinstance(container_image, ImageSpec):
+            if container_image.base_image is None:
+                img = f"cr.flyte.org/flyteorg/flytekit:spark-{DefaultImages.get_version_suffix()}"
+                container_image.base_image = img
+                # default executor path and applications path in apache/spark-py:3.3.1
+                self._default_executor_path = "/usr/bin/python3"
+                self._default_applications_path = "local:///usr/local/bin/entrypoint.py"
         super(PysparkFunctionTask, self).__init__(
             task_config=task_config,
             task_type=self._SPARK_TASK_TYPE,
             task_function=task_function,
+            container_image=container_image,
             **kwargs,
         )
-        self.sess: Optional[SparkSession] = None
 
     def get_custom(self, settings: SerializationSettings) -> Dict[str, Any]:
         job = SparkJob(
             spark_conf=self.task_config.spark_conf,
             hadoop_conf=self.task_config.hadoop_conf,
-            application_file="local://" + settings.entrypoint_settings.path,
-            executor_path=settings.python_interpreter,
+            application_file=self._default_applications_path or "local://" + settings.entrypoint_settings.path,
+            executor_path=self._default_executor_path or settings.python_interpreter,
             main_class="",
             spark_type=SparkType.PYTHON,
         )
         if isinstance(self.task_config, Databricks):
-            cfg = typing.cast(Databricks, self.task_config)
+            cfg = cast(Databricks, self.task_config)
             job._databricks_conf = cfg.databricks_conf
             job._databricks_token = cfg.databricks_token
             job._databricks_instance = cfg.databricks_instance
 
         return MessageToDict(job.to_flyte_idl())
 
     def pre_execute(self, user_params: ExecutionParameters) -> ExecutionParameters:
```

### Comparing `flytekitplugins-spark-1.6.0b1/flytekitplugins_spark.egg-info/PKG-INFO` & `flytekitplugins-spark-1.6.0b2/flytekitplugins_spark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-spark
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: Spark 3 plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-spark-1.6.0b1/flytekitplugins_spark.egg-info/SOURCES.txt` & `flytekitplugins-spark-1.6.0b2/flytekitplugins_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b1/scripts/flytekit_install_spark3.sh` & `flytekitplugins-spark-1.6.0b2/scripts/flytekit_install_spark3.sh`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b1/setup.py` & `flytekitplugins-spark-1.6.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "spark"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "pyspark>=3.0.0"]
 
-__version__ = "1.6.0b1"
+__version__ = "1.6.0b2"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="Spark 3 plugin for flytekit",
```

