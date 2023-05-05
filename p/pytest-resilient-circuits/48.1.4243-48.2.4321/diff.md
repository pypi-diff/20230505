# Comparing `tmp/pytest_resilient_circuits-48.1.4243.tar.gz` & `tmp/pytest_resilient_circuits-48.2.4321.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_resilient_circuits-48.1.4243.tar", last modified: Thu Apr 20 19:35:39 2023, max compression
+gzip compressed data, was "pytest_resilient_circuits-48.2.4321.tar", last modified: Fri May  5 12:35:24 2023, max compression
```

## Comparing `pytest_resilient_circuits-48.1.4243.tar` & `pytest_resilient_circuits-48.2.4321.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:39.315501 pytest_resilient_circuits-48.1.4243/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10889 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2210 2023-04-20 19:35:39.315501 pytest_resilient_circuits-48.1.4243/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1447 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:39.311501 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      370 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4090 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/circuits_fixtures.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:39.311501 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      604 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__actions.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1025 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__attachments.json
--rw-rw-r--   0 travis    (2000) travis    (2000)   282455 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__const.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      798 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__functions.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3087 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__incidents_2314.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      400 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__message_destinations.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1459 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__task.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      775 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__types_artifact.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3527 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__types_function_fields.json
--rw-rw-r--   0 travis    (2000) travis    (2000)   180619 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__types_incident_fields.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      580 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__wiki100.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      604 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__wiki3.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      501 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__wikis.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      428 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_POST__attachment.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      359 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_POST__table_data.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      542 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/misc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18019 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/mocks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1954 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/plugin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22326 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/resilient_circuits_fixtures.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:39.311501 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/shared_mock_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      387 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/shared_mock_data/mock_constants.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:39.311501 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2210 2023-04-20 19:35:39.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1696 2023-04-20 19:35:39.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:35:39.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       72 2023-04-20 19:35:39.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      160 2023-04-20 19:35:39.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       26 2023-04-20 19:35:39.000000 pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2023-04-20 19:35:39.315501 pytest_resilient_circuits-48.1.4243/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      196 2023-04-20 19:34:28.000000 pytest_resilient_circuits-48.1.4243/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:24.883470 pytest_resilient_circuits-48.2.4321/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10889 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2210 2023-05-05 12:35:24.883470 pytest_resilient_circuits-48.2.4321/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1447 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:24.879470 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      370 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4090 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/circuits_fixtures.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:24.883470 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      604 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__actions.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1025 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__attachments.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)   282455 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__const.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      798 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__functions.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3087 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__incidents_2314.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      400 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__message_destinations.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1459 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__task.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      775 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__types_artifact.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3527 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__types_function_fields.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)   180619 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__types_incident_fields.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      580 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__wiki100.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      604 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__wiki3.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      501 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__wikis.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      428 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_POST__attachment.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      359 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_POST__table_data.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      542 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/misc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18019 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/mocks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1954 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/plugin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22326 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/resilient_circuits_fixtures.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:24.883470 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/shared_mock_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      387 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/shared_mock_data/mock_constants.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:24.879470 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2210 2023-05-05 12:35:24.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1696 2023-05-05 12:35:24.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:35:24.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       72 2023-05-05 12:35:24.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      160 2023-05-05 12:35:24.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       26 2023-05-05 12:35:24.000000 pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2023-05-05 12:35:24.883470 pytest_resilient_circuits-48.2.4321/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      196 2023-05-05 12:33:36.000000 pytest_resilient_circuits-48.2.4321/setup.py
```

### Comparing `pytest_resilient_circuits-48.1.4243/CHANGES` & `pytest_resilient_circuits-48.2.4321/CHANGES`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-48.1.4243/PKG-INFO` & `pytest_resilient_circuits-48.2.4321/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_resilient_circuits
-Version: 48.1.4243
+Version: 48.2.4321
 Summary: Resilient Circuits fixtures for PyTest
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-resilient-circuits
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `pytest_resilient_circuits-48.1.4243/README.md` & `pytest_resilient_circuits-48.2.4321/README.md`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/LICENSE` & `pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/circuits_fixtures.py` & `pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/circuits_fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__actions.json` & `pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__actions.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__attachments.json` & `pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__attachments.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__const.json` & `pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__const.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__functions.json` & `pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__functions.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__incidents_2314.json` & `pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__incidents_2314.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__task.json` & `pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__task.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__types_artifact.json` & `pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__types_artifact.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__types_function_fields.json` & `pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__types_function_fields.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__types_incident_fields.json` & `pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__types_incident_fields.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__wiki100.json` & `pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__wiki100.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/data/200_JSON_GET__wiki3.json` & `pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/data/200_JSON_GET__wiki3.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/misc.py` & `pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/misc.py`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/mocks.py` & `pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/mocks.py`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/plugin.py` & `pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits/resilient_circuits_fixtures.py` & `pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits/resilient_circuits_fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits.egg-info/PKG-INFO` & `pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-resilient-circuits
-Version: 48.1.4243
+Version: 48.2.4321
 Summary: Resilient Circuits fixtures for PyTest
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-resilient-circuits
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `pytest_resilient_circuits-48.1.4243/pytest_resilient_circuits.egg-info/SOURCES.txt` & `pytest_resilient_circuits-48.2.4321/pytest_resilient_circuits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-48.1.4243/setup.cfg` & `pytest_resilient_circuits-48.2.4321/setup.cfg`

 * *Files identical despite different names*

