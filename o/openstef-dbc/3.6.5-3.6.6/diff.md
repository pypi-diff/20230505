# Comparing `tmp/openstef_dbc-3.6.5.tar.gz` & `tmp/openstef_dbc-3.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstef_dbc-3.6.5.tar", last modified: Thu May  4 08:41:30 2023, max compression
+gzip compressed data, was "openstef_dbc-3.6.6.tar", last modified: Fri May  5 12:22:08 2023, max compression
```

## Comparing `openstef_dbc-3.6.5.tar` & `openstef_dbc-3.6.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:41:30.490763 openstef_dbc-3.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-04 08:41:30.490763 openstef_dbc-3.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:41:30.490763 openstef_dbc-3.6.5/openstef_dbc/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/data_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/ktp_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:41:30.490763 openstef_dbc-3.6.5/openstef_dbc/log/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/log/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/log/processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:41:30.490763 openstef_dbc-3.6.5/openstef_dbc/models/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/models/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/models/switch_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:41:30.490763 openstef_dbc-3.6.5/openstef_dbc/services/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/services/ems.py
--rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/services/model_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/services/prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/services/predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/services/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/services/splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/services/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/services/weather.py
--rw-r--r--   0 runner    (1001) docker     (123)    15440 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/services/write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/openstef_dbc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:41:30.490763 openstef_dbc-3.6.5/openstef_dbc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-04 08:41:30.000000 openstef_dbc-3.6.5/openstef_dbc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-04 08:41:30.000000 openstef_dbc-3.6.5/openstef_dbc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:41:30.000000 openstef_dbc-3.6.5/openstef_dbc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-04 08:41:30.000000 openstef_dbc-3.6.5/openstef_dbc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 08:41:30.000000 openstef_dbc-3.6.5/openstef_dbc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-04 08:41:30.490763 openstef_dbc-3.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-04 08:41:18.000000 openstef_dbc-3.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:08.284922 openstef_dbc-3.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-05 12:22:08.284922 openstef_dbc-3.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:08.280923 openstef_dbc-3.6.6/openstef_dbc/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/data_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/ktp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:08.280923 openstef_dbc-3.6.6/openstef_dbc/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/log/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/log/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:08.280923 openstef_dbc-3.6.6/openstef_dbc/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/models/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/models/switch_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:08.284922 openstef_dbc-3.6.6/openstef_dbc/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/services/ems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/services/model_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/services/prediction_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/services/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/services/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/services/splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/services/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/services/weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/services/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:08.280923 openstef_dbc-3.6.6/openstef_dbc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-05 12:22:08.000000 openstef_dbc-3.6.6/openstef_dbc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-05 12:22:08.000000 openstef_dbc-3.6.6/openstef_dbc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:22:08.000000 openstef_dbc-3.6.6/openstef_dbc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-05 12:22:08.000000 openstef_dbc-3.6.6/openstef_dbc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 12:22:08.000000 openstef_dbc-3.6.6/openstef_dbc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-05 12:22:08.284922 openstef_dbc-3.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/setup.py
```

### Comparing `openstef_dbc-3.6.5/LICENSE` & `openstef_dbc-3.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.5/PKG-INFO` & `openstef_dbc-3.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef_dbc
-Version: 3.6.5
+Version: 3.6.6
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openstef_dbc-3.6.5/README.md` & `openstef_dbc-3.6.6/README.md`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.5/openstef_dbc/__init__.py` & `openstef_dbc-3.6.6/openstef_dbc/__init__.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.5/openstef_dbc/data_interface.py` & `openstef_dbc-3.6.6/openstef_dbc/data_interface.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.5/openstef_dbc/database.py` & `openstef_dbc-3.6.6/openstef_dbc/database.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.5/openstef_dbc/ktp_api.py` & `openstef_dbc-3.6.6/openstef_dbc/ktp_api.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.5/openstef_dbc/log/logging.py` & `openstef_dbc-3.6.6/openstef_dbc/log/logging.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.5/openstef_dbc/log/processors.py` & `openstef_dbc-3.6.6/openstef_dbc/log/processors.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.5/openstef_dbc/models/measurement.py` & `openstef_dbc-3.6.6/openstef_dbc/models/measurement.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.5/openstef_dbc/services/ems.py` & `openstef_dbc-3.6.6/openstef_dbc/services/ems.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.5/openstef_dbc/services/model_input.py` & `openstef_dbc-3.6.6/openstef_dbc/services/model_input.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.5/openstef_dbc/services/prediction_job.py` & `openstef_dbc-3.6.6/openstef_dbc/services/prediction_job.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.5/openstef_dbc/services/predictions.py` & `openstef_dbc-3.6.6/openstef_dbc/services/predictions.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.5/openstef_dbc/services/predictor.py` & `openstef_dbc-3.6.6/openstef_dbc/services/predictor.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.5/openstef_dbc/services/splitting.py` & `openstef_dbc-3.6.6/openstef_dbc/services/splitting.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.5/openstef_dbc/services/systems.py` & `openstef_dbc-3.6.6/openstef_dbc/services/systems.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.5/openstef_dbc/services/weather.py` & `openstef_dbc-3.6.6/openstef_dbc/services/weather.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.5/openstef_dbc/services/write.py` & `openstef_dbc-3.6.6/openstef_dbc/services/write.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         forecast["created"] = int(datetime.utcnow().timestamp())
 
         # Add quality column. Fill nan's or missing column with 'actual'
         if force_quality:
             if "quality" not in forecast.columns:
                 forecast["quality"] = "actual"
             else:
-                forecast[forecast["quality"].isna()] = "actual"
+                forecast.loc[forecast["quality"].isna(), "quality"] = "actual"
 
         # Write DataFrame to influx database
         # Find tag columns
         tag_columns = ["pid", "type", "customer"]
         # Specify field columns
         field_columns = [x for x in forecast.columns if x not in tag_columns]
```

### Comparing `openstef_dbc-3.6.5/openstef_dbc/utils.py` & `openstef_dbc-3.6.6/openstef_dbc/utils.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.5/openstef_dbc.egg-info/PKG-INFO` & `openstef_dbc-3.6.6/openstef_dbc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef-dbc
-Version: 3.6.5
+Version: 3.6.6
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openstef_dbc-3.6.5/openstef_dbc.egg-info/SOURCES.txt` & `openstef_dbc-3.6.6/openstef_dbc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.5/setup.py` & `openstef_dbc-3.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def read_long_description_from_readme():
     with open("README.md", "r", encoding="utf-8") as fh:
         return fh.read()
 
 
 setup(
     name="openstef_dbc",
-    version="3.6.5",
+    version="3.6.6",
     packages=find_packages(include=["openstef_dbc", "openstef_dbc.*"]),
     description="Database Connection for OpenSTEF",
     long_description=read_long_description_from_readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/openstef/openstef-dbc",
     author="Alliander N.V",
     author_email="korte.termijn.prognoses@alliander.com",
```

