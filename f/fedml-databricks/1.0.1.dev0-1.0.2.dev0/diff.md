# Comparing `tmp/fedml_databricks-1.0.1.dev0.tar.gz` & `tmp/fedml_databricks-1.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedml_databricks-1.0.1.dev0.tar", last modified: Wed Feb  1 21:49:49 2023, max compression
+gzip compressed data, was "fedml_databricks-1.0.2.dev0.tar", last modified: Thu May  4 21:50:09 2023, max compression
```

## Comparing `fedml_databricks-1.0.1.dev0.tar` & `fedml_databricks-1.0.2.dev0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-02-01 21:49:49.021806 fedml_databricks-1.0.1.dev0/
--rw-r--r--   0 I550585    (501) staff       (20)    11307 2023-02-01 00:25:27.000000 fedml_databricks-1.0.1.dev0/LICENSE.txt
--rw-r--r--   0 I550585    (501) staff       (20)     1358 2023-02-01 21:49:49.021134 fedml_databricks-1.0.1.dev0/PKG-INFO
--rw-r--r--   0 I550585    (501) staff       (20)      960 2023-02-01 00:25:27.000000 fedml_databricks-1.0.1.dev0/README.md
--rw-r--r--   0 I550585    (501) staff       (20)      103 2023-02-01 00:25:03.000000 fedml_databricks-1.0.1.dev0/pyproject.toml
--rw-r--r--   0 I550585    (501) staff       (20)       38 2023-02-01 21:49:49.021959 fedml_databricks-1.0.1.dev0/setup.cfg
--rw-r--r--   0 I550585    (501) staff       (20)     1102 2023-02-01 21:40:59.000000 fedml_databricks-1.0.1.dev0/setup.py
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-02-01 21:49:48.944617 fedml_databricks-1.0.1.dev0/src/
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-02-01 21:49:48.979360 fedml_databricks-1.0.1.dev0/src/fedml_databricks/
--rw-r--r--   0 I550585    (501) staff       (20)      107 2023-02-01 00:25:27.000000 fedml_databricks-1.0.1.dev0/src/fedml_databricks/__init__.py
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-02-01 21:49:49.002700 fedml_databricks-1.0.1.dev0/src/fedml_databricks/acr/
--rw-r--r--   0 I550585    (501) staff       (20)        0 2023-02-01 00:25:27.000000 fedml_databricks-1.0.1.dev0/src/fedml_databricks/acr/__init__.py
--rw-r--r--   0 I550585    (501) staff       (20)     1694 2023-02-01 19:09:31.000000 fedml_databricks-1.0.1.dev0/src/fedml_databricks/acr/acr_kyma_deploy.py
--rw-r--r--   0 I550585    (501) staff       (20)     6823 2023-02-01 01:19:55.000000 fedml_databricks-1.0.1.dev0/src/fedml_databricks/acr/acr_kyma_deploy.sh
--rw-r--r--   0 I550585    (501) staff       (20)      332 2023-02-01 00:25:27.000000 fedml_databricks-1.0.1.dev0/src/fedml_databricks/databricks_cli_configure.sh
--rw-r--r--   0 I550585    (501) staff       (20)    15322 2023-02-01 00:25:27.000000 fedml_databricks-1.0.1.dev0/src/fedml_databricks/dbconnection.py
--rw-r--r--   0 I550585    (501) staff       (20)      682 2023-02-01 00:25:27.000000 fedml_databricks-1.0.1.dev0/src/fedml_databricks/deployment_helper.py
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-02-01 21:49:49.019942 fedml_databricks-1.0.1.dev0/src/fedml_databricks/ecr/
--rw-r--r--   0 I550585    (501) staff       (20)        0 2023-02-01 00:25:27.000000 fedml_databricks-1.0.1.dev0/src/fedml_databricks/ecr/__init__.py
--rw-r--r--   0 I550585    (501) staff       (20)     1597 2023-02-01 00:55:43.000000 fedml_databricks-1.0.1.dev0/src/fedml_databricks/ecr/ecr_kyma_deploy.py
--rw-r--r--   0 I550585    (501) staff       (20)     5006 2023-02-01 00:25:27.000000 fedml_databricks-1.0.1.dev0/src/fedml_databricks/ecr/ecr_kyma_deploy.sh
--rw-r--r--   0 I550585    (501) staff       (20)     1771 2023-02-01 00:25:27.000000 fedml_databricks-1.0.1.dev0/src/fedml_databricks/kubectl_install_validate.sh
--rw-r--r--   0 I550585    (501) staff       (20)     3909 2023-02-01 00:25:27.000000 fedml_databricks-1.0.1.dev0/src/fedml_databricks/kyma_deploy.py
--rw-r--r--   0 I550585    (501) staff       (20)      656 2023-02-01 00:25:03.000000 fedml_databricks-1.0.1.dev0/src/fedml_databricks/logger.py
--rw-r--r--   0 I550585    (501) staff       (20)      701 2023-02-01 21:38:38.000000 fedml_databricks-1.0.1.dev0/src/fedml_databricks/predict.py
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-02-01 21:49:48.985633 fedml_databricks-1.0.1.dev0/src/fedml_databricks.egg-info/
--rw-r--r--   0 I550585    (501) staff       (20)     1358 2023-02-01 21:49:48.000000 fedml_databricks-1.0.1.dev0/src/fedml_databricks.egg-info/PKG-INFO
--rw-r--r--   0 I550585    (501) staff       (20)      823 2023-02-01 21:49:48.000000 fedml_databricks-1.0.1.dev0/src/fedml_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 I550585    (501) staff       (20)        1 2023-02-01 21:49:48.000000 fedml_databricks-1.0.1.dev0/src/fedml_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 I550585    (501) staff       (20)       65 2023-02-01 21:49:48.000000 fedml_databricks-1.0.1.dev0/src/fedml_databricks.egg-info/requires.txt
--rw-r--r--   0 I550585    (501) staff       (20)       17 2023-02-01 21:49:48.000000 fedml_databricks-1.0.1.dev0/src/fedml_databricks.egg-info/top_level.txt
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-04 21:50:09.681326 fedml_databricks-1.0.2.dev0/
+-rw-r--r--   0 I550585    (501) staff       (20)    11307 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/LICENSE.txt
+-rw-r--r--   0 I550585    (501) staff       (20)     1348 2023-05-04 21:50:09.680856 fedml_databricks-1.0.2.dev0/PKG-INFO
+-rw-r--r--   0 I550585    (501) staff       (20)      950 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/README.md
+-rw-r--r--   0 I550585    (501) staff       (20)      103 2023-02-01 00:25:03.000000 fedml_databricks-1.0.2.dev0/pyproject.toml
+-rw-r--r--   0 I550585    (501) staff       (20)       38 2023-05-04 21:50:09.681448 fedml_databricks-1.0.2.dev0/setup.cfg
+-rw-r--r--   0 I550585    (501) staff       (20)     1102 2023-05-04 21:49:36.000000 fedml_databricks-1.0.2.dev0/setup.py
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-04 21:50:09.589121 fedml_databricks-1.0.2.dev0/src/
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-04 21:50:09.641988 fedml_databricks-1.0.2.dev0/src/fedml_databricks/
+-rw-r--r--   0 I550585    (501) staff       (20)      107 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/__init__.py
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-04 21:50:09.662997 fedml_databricks-1.0.2.dev0/src/fedml_databricks/acr/
+-rw-r--r--   0 I550585    (501) staff       (20)        0 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/acr/__init__.py
+-rw-r--r--   0 I550585    (501) staff       (20)     1694 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/acr/acr_kyma_deploy.py
+-rw-r--r--   0 I550585    (501) staff       (20)     6823 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/acr/acr_kyma_deploy.sh
+-rw-r--r--   0 I550585    (501) staff       (20)      332 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/databricks_cli_configure.sh
+-rw-r--r--   0 I550585    (501) staff       (20)    15603 2023-05-03 23:57:50.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/dbconnection.py
+-rw-r--r--   0 I550585    (501) staff       (20)      682 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/deployment_helper.py
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-04 21:50:09.679934 fedml_databricks-1.0.2.dev0/src/fedml_databricks/ecr/
+-rw-r--r--   0 I550585    (501) staff       (20)        0 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/ecr/__init__.py
+-rw-r--r--   0 I550585    (501) staff       (20)     1597 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/ecr/ecr_kyma_deploy.py
+-rw-r--r--   0 I550585    (501) staff       (20)     5006 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/ecr/ecr_kyma_deploy.sh
+-rw-r--r--   0 I550585    (501) staff       (20)     1771 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/kubectl_install_validate.sh
+-rw-r--r--   0 I550585    (501) staff       (20)     3909 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/kyma_deploy.py
+-rw-r--r--   0 I550585    (501) staff       (20)      656 2023-02-01 00:25:03.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/logger.py
+-rw-r--r--   0 I550585    (501) staff       (20)      701 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/predict.py
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-04 21:50:09.646464 fedml_databricks-1.0.2.dev0/src/fedml_databricks.egg-info/
+-rw-r--r--   0 I550585    (501) staff       (20)     1348 2023-05-04 21:50:09.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 I550585    (501) staff       (20)      823 2023-05-04 21:50:09.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 I550585    (501) staff       (20)        1 2023-05-04 21:50:09.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 I550585    (501) staff       (20)       65 2023-05-04 21:50:09.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks.egg-info/requires.txt
+-rw-r--r--   0 I550585    (501) staff       (20)       17 2023-05-04 21:50:09.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks.egg-info/top_level.txt
```

### Comparing `fedml_databricks-1.0.1.dev0/LICENSE.txt` & `fedml_databricks-1.0.2.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.1.dev0/PKG-INFO` & `fedml_databricks-1.0.2.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fedml_databricks
-Version: 1.0.1.dev0
+Version: 1.0.2.dev0
 Summary: A python library for building machine learning models on Databricks using a federated data source
 Author: SAP SE
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ## Introduction
 
-The SAP Federated ML Python library for Databricks applies the Data Federation architecture of SAP Data Warehouse Cloud for intelligently sourcing SAP as well as non-SAP data for Machine Learning experiments done in Databricks, thereby removing the need for replicating or moving the data. By abstracting the Data Connection, Data load, Model Deployment in SAP environment, and Inferencing for Machine learning processes , the FedML Databricks library provides end to end integration with few lines of code.
+The SAP Federated ML Python library for Databricks applies the Data Federation architecture of SAP Datasphere for intelligently sourcing SAP as well as non-SAP data for Machine Learning experiments done in Databricks, thereby removing the need for replicating or moving the data. By abstracting the Data Connection, Data load, Model Deployment in SAP environment, and Inferencing for Machine learning processes , the FedML Databricks library provides end to end integration with few lines of code.
 
 ## Installation
 
 Install the SAP FedML Databricks library using pip as follows:
 
 `pip install fedml-databricks --no-cache-dir --upgrade --force-reinstall`
```

### Comparing `fedml_databricks-1.0.1.dev0/README.md` & `fedml_databricks-1.0.2.dev0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ## Introduction
 
-The SAP Federated ML Python library for Databricks applies the Data Federation architecture of SAP Data Warehouse Cloud for intelligently sourcing SAP as well as non-SAP data for Machine Learning experiments done in Databricks, thereby removing the need for replicating or moving the data. By abstracting the Data Connection, Data load, Model Deployment in SAP environment, and Inferencing for Machine learning processes , the FedML Databricks library provides end to end integration with few lines of code.
+The SAP Federated ML Python library for Databricks applies the Data Federation architecture of SAP Datasphere for intelligently sourcing SAP as well as non-SAP data for Machine Learning experiments done in Databricks, thereby removing the need for replicating or moving the data. By abstracting the Data Connection, Data load, Model Deployment in SAP environment, and Inferencing for Machine learning processes , the FedML Databricks library provides end to end integration with few lines of code.
 
 ## Installation
 
 Install the SAP FedML Databricks library using pip as follows:
 
 `pip install fedml-databricks --no-cache-dir --upgrade --force-reinstall`
```

### Comparing `fedml_databricks-1.0.1.dev0/setup.py` & `fedml_databricks-1.0.2.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setuptools.setup(
     name="fedml_databricks",
-    version="1.0.1.dev0",
+    version="1.0.2.dev0",
     author="SAP SE",
     description="A python library for building machine learning models on Databricks using a federated data source",
     license='Apache License 2.0',
     license_files = ['LICENSE.txt'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
```

### Comparing `fedml_databricks-1.0.1.dev0/src/fedml_databricks/acr/acr_kyma_deploy.py` & `fedml_databricks-1.0.2.dev0/src/fedml_databricks/acr/acr_kyma_deploy.py`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.1.dev0/src/fedml_databricks/acr/acr_kyma_deploy.sh` & `fedml_databricks-1.0.2.dev0/src/fedml_databricks/acr/acr_kyma_deploy.sh`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.1.dev0/src/fedml_databricks/dbconnection.py` & `fedml_databricks-1.0.2.dev0/src/fedml_databricks/dbconnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
             self.connection.rollback()
             raise
     
     def get_data_with_headers_pyspark(self, table_name, size=1):
         try:
             data,column_headers=self.get_data_with_headers(table_name,size)
         except Exception as e:
-            self.logger.error('error occured during query executionk %s', e)
+            self.logger.error('error occured during query execution. %s', e)
             self.connection.rollback()
             raise
         try:
             pandas_df=pd.DataFrame(data, columns=column_headers)
             spark = SparkSession.builder.getOrCreate()
             spark_df = spark.createDataFrame(data=pandas_df)
             return spark_df
@@ -136,37 +136,39 @@
     def execute_query(self, query):
         if (self.connection.isconnected()):
             cursor = self.connection.cursor()
         else:
             self._get_connection()
             cursor = self.connection.cursor()
         try:
+            if query.split()[0].lower()!="select":
+                raise Exception("The ‘execute_query’ and ‘execute_query_pyspark’ methods supports ‘select’ SQL statements only. For other SQL statements, use the appropriate methods by referring the documentation.")
             cursor.execute(query)
             res = cursor.fetchall()
             column_headers = [i[0] for i in cursor.description]
             return res, column_headers
         except Exception as e:
-            self.logger.error('error occured during query execution %s', e)
+            self.logger.error('error occured during query execution: %s', e)
             self.connection.rollback()
             raise
     
     def execute_query_pyspark(self, query):
         try:
             data,column_headers=self.execute_query(query)
         except Exception as e:
-            self.logger.error('error occured during query execution %s', e)
+            self.logger.error('error occured during query execution: %s', e)
             self.connection.rollback()
             raise
         try:
             pandas_df=pd.DataFrame(data, columns=column_headers)
             spark = SparkSession.builder.getOrCreate()
             spark_df = spark.createDataFrame(data=pandas_df)
             return spark_df
         except Exception as e:
-            self.logger.error('error occured while retrieving the data as PySpark dataframe.Use the "execute_query" method to get the data. %s', e)
+            self.logger.error('error occured while retrieving the data as PySpark dataframe.Use the "execute_query" method to get the data: %s', e)
             self.connection.rollback()
             raise
 
     def create_table(self, query):
         if (self.connection.isconnected()):
             cursor = self.connection.cursor()
         else:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fedml_databricks-1.0.1.dev0/src/fedml_databricks/deployment_helper.py` & `fedml_databricks-1.0.2.dev0/src/fedml_databricks/deployment_helper.py`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.1.dev0/src/fedml_databricks/ecr/ecr_kyma_deploy.py` & `fedml_databricks-1.0.2.dev0/src/fedml_databricks/ecr/ecr_kyma_deploy.py`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.1.dev0/src/fedml_databricks/ecr/ecr_kyma_deploy.sh` & `fedml_databricks-1.0.2.dev0/src/fedml_databricks/ecr/ecr_kyma_deploy.sh`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.1.dev0/src/fedml_databricks/kubectl_install_validate.sh` & `fedml_databricks-1.0.2.dev0/src/fedml_databricks/kubectl_install_validate.sh`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.1.dev0/src/fedml_databricks/kyma_deploy.py` & `fedml_databricks-1.0.2.dev0/src/fedml_databricks/kyma_deploy.py`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.1.dev0/src/fedml_databricks/logger.py` & `fedml_databricks-1.0.2.dev0/src/fedml_databricks/logger.py`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.1.dev0/src/fedml_databricks/predict.py` & `fedml_databricks-1.0.2.dev0/src/fedml_databricks/predict.py`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.1.dev0/src/fedml_databricks.egg-info/PKG-INFO` & `fedml_databricks-1.0.2.dev0/src/fedml_databricks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fedml-databricks
-Version: 1.0.1.dev0
+Version: 1.0.2.dev0
 Summary: A python library for building machine learning models on Databricks using a federated data source
 Author: SAP SE
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ## Introduction
 
-The SAP Federated ML Python library for Databricks applies the Data Federation architecture of SAP Data Warehouse Cloud for intelligently sourcing SAP as well as non-SAP data for Machine Learning experiments done in Databricks, thereby removing the need for replicating or moving the data. By abstracting the Data Connection, Data load, Model Deployment in SAP environment, and Inferencing for Machine learning processes , the FedML Databricks library provides end to end integration with few lines of code.
+The SAP Federated ML Python library for Databricks applies the Data Federation architecture of SAP Datasphere for intelligently sourcing SAP as well as non-SAP data for Machine Learning experiments done in Databricks, thereby removing the need for replicating or moving the data. By abstracting the Data Connection, Data load, Model Deployment in SAP environment, and Inferencing for Machine learning processes , the FedML Databricks library provides end to end integration with few lines of code.
 
 ## Installation
 
 Install the SAP FedML Databricks library using pip as follows:
 
 `pip install fedml-databricks --no-cache-dir --upgrade --force-reinstall`
```

### Comparing `fedml_databricks-1.0.1.dev0/src/fedml_databricks.egg-info/SOURCES.txt` & `fedml_databricks-1.0.2.dev0/src/fedml_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

