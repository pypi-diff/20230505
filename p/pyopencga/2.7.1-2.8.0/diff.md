# Comparing `tmp/pyopencga-2.7.1.tar.gz` & `tmp/pyopencga-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopencga-2.7.1.tar", last modified: Thu Mar 23 12:40:57 2023, max compression
+gzip compressed data, was "pyopencga-2.8.0.tar", last modified: Tue Apr 25 17:34:32 2023, max compression
```

## Comparing `pyopencga-2.7.1.tar` & `pyopencga-2.8.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:40:57.143165 pyopencga-2.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-23 12:40:23.000000 pyopencga-2.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-03-23 12:40:57.143165 pyopencga-2.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-03-23 12:40:23.000000 pyopencga-2.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:40:57.131165 pyopencga-2.7.1/pyopencga/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-23 12:40:23.000000 pyopencga-2.7.1/pyopencga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-03-23 12:40:23.000000 pyopencga-2.7.1/pyopencga/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-23 12:40:23.000000 pyopencga-2.7.1/pyopencga/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/opencga_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/opencga_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:40:57.143165 pyopencga-2.7.1/pyopencga/rest_clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_clients/_parent_rest_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_clients/admin_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_clients/alignment_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52180 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_clients/clinical_analysis_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52556 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_clients/clinical_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14958 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_clients/cohort_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_clients/disease_panel_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15190 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_clients/family_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26679 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_clients/file_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_clients/ga4gh_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18059 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_clients/individual_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13142 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_clients/job_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_clients/meta_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_clients/project_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19724 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_clients/sample_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17217 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_clients/study_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_clients/user_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    61388 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_clients/variant_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25730 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_clients/variant_operation_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/rest_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-03-23 12:40:24.000000 pyopencga-2.7.1/pyopencga/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:40:57.135165 pyopencga-2.7.1/pyopencga.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-03-23 12:40:57.000000 pyopencga-2.7.1/pyopencga.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-03-23 12:40:57.000000 pyopencga-2.7.1/pyopencga.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 12:40:57.000000 pyopencga-2.7.1/pyopencga.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-23 12:40:57.000000 pyopencga-2.7.1/pyopencga.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-23 12:40:57.000000 pyopencga-2.7.1/pyopencga.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 12:40:57.143165 pyopencga-2.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-03-23 12:40:23.000000 pyopencga-2.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:34:32.948865 pyopencga-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-25 17:34:01.000000 pyopencga-2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-25 17:34:32.948865 pyopencga-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-04-25 17:34:01.000000 pyopencga-2.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:34:32.944865 pyopencga-2.8.0/pyopencga/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/opencga_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/opencga_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:34:32.948865 pyopencga-2.8.0/pyopencga/rest_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/_parent_rest_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/alignment_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52128 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/clinical_analysis_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52556 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/clinical_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/cohort_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/disease_panel_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/family_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26628 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/file_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/ga4gh_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18007 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_clients/individual_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-04-25 17:34:03.000000 pyopencga-2.8.0/pyopencga/rest_clients/job_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-25 17:34:03.000000 pyopencga-2.8.0/pyopencga/rest_clients/meta_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-04-25 17:34:03.000000 pyopencga-2.8.0/pyopencga/rest_clients/project_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-04-25 17:34:03.000000 pyopencga-2.8.0/pyopencga/rest_clients/sample_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-04-25 17:34:03.000000 pyopencga-2.8.0/pyopencga/rest_clients/study_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-04-25 17:34:03.000000 pyopencga-2.8.0/pyopencga/rest_clients/user_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61336 2023-04-25 17:34:03.000000 pyopencga-2.8.0/pyopencga/rest_clients/variant_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25700 2023-04-25 17:34:03.000000 pyopencga-2.8.0/pyopencga/rest_clients/variant_operation_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/rest_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-25 17:34:02.000000 pyopencga-2.8.0/pyopencga/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:34:32.944865 pyopencga-2.8.0/pyopencga.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-25 17:34:32.000000 pyopencga-2.8.0/pyopencga.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-25 17:34:32.000000 pyopencga-2.8.0/pyopencga.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 17:34:32.000000 pyopencga-2.8.0/pyopencga.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 17:34:32.000000 pyopencga-2.8.0/pyopencga.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 17:34:32.000000 pyopencga-2.8.0/pyopencga.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 17:34:32.948865 pyopencga-2.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-25 17:34:01.000000 pyopencga-2.8.0/setup.py
```

### Comparing `pyopencga-2.7.1/LICENSE` & `pyopencga-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopencga-2.7.1/PKG-INFO` & `pyopencga-2.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencga
-Version: 2.7.1
+Version: 2.8.0
 Summary: A REST client for OpenCGA REST web services
 Home-page: https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga
 Author: David Gomez-Peregrina, Pablo Marin-Garcia, Daniel Perez-Gil
 Author-email: david.gomez@mgviz.org, pmarin@kanteron.com, dp529@cam.ac.uk
 License: Apache Software License
 Project-URL: Documentation, http://docs.opencb.org/display/opencga/Python
 Project-URL: Source, https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga
```

### Comparing `pyopencga-2.7.1/README.rst` & `pyopencga-2.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyopencga-2.7.1/pyopencga/commons.py` & `pyopencga-2.8.0/pyopencga/commons.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.7.1/pyopencga/opencga_client.py` & `pyopencga-2.8.0/pyopencga/opencga_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.7.1/pyopencga/opencga_config.py` & `pyopencga-2.8.0/pyopencga/opencga_config.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.7.1/pyopencga/rest_clients/_parent_rest_clients.py` & `pyopencga-2.8.0/pyopencga/rest_clients/_parent_rest_clients.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.7.1/pyopencga/rest_clients/admin_client.py` & `pyopencga-2.8.0/pyopencga/rest_clients/admin_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-01-10 10:57:29
+    Autogenerated on: 2023-04-18
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Admin(_ParentRestClient):
     """
     This class contains methods for the 'Admin' webservices
-    Client version: 2.6.0-SNAPSHOT [cd4c96caf1cb7afcdec5f54a7de72bde4f63820e]
+    Client version: 2.8.0-SNAPSHOT
     PATH: /{apiVersion}/admin
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Admin, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def group_by_audit(self, fields, entity, **options):
```

### Comparing `pyopencga-2.7.1/pyopencga/rest_clients/alignment_client.py` & `pyopencga-2.8.0/pyopencga/rest_clients/alignment_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-01-10 10:57:29
+    Autogenerated on: 2023-04-18
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Alignment(_ParentRestClient):
     """
     This class contains methods for the 'Analysis - Alignment' webservices
-    Client version: 2.6.0-SNAPSHOT [cd4c96caf1cb7afcdec5f54a7de72bde4f63820e]
+    Client version: 2.8.0-SNAPSHOT
     PATH: /{apiVersion}/analysis/alignment
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Alignment, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def run_bwa(self, data=None, **options):
```

### Comparing `pyopencga-2.7.1/pyopencga/rest_clients/clinical_analysis_client.py` & `pyopencga-2.8.0/pyopencga/rest_clients/clinical_analysis_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-01-10 10:57:29
+    Autogenerated on: 2023-04-18
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class ClinicalAnalysis(_ParentRestClient):
     """
     This class contains methods for the 'Analysis - Clinical' webservices
-    Client version: 2.6.0-SNAPSHOT [cd4c96caf1cb7afcdec5f54a7de72bde4f63820e]
+    Client version: 2.8.0-SNAPSHOT
     PATH: /{apiVersion}/analysis/clinical
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(ClinicalAnalysis, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
```

### Comparing `pyopencga-2.7.1/pyopencga/rest_clients/clinical_client.py` & `pyopencga-2.8.0/pyopencga/rest_clients/clinical_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.7.1/pyopencga/rest_clients/cohort_client.py` & `pyopencga-2.8.0/pyopencga/rest_clients/cohort_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-01-10 10:57:29
+    Autogenerated on: 2023-04-18
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Cohort(_ParentRestClient):
     """
     This class contains methods for the 'Cohorts' webservices
-    Client version: 2.6.0-SNAPSHOT [cd4c96caf1cb7afcdec5f54a7de72bde4f63820e]
+    Client version: 2.8.0-SNAPSHOT
     PATH: /{apiVersion}/cohorts
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Cohort, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
```

### Comparing `pyopencga-2.7.1/pyopencga/rest_clients/disease_panel_client.py` & `pyopencga-2.8.0/pyopencga/rest_clients/disease_panel_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-01-10 10:57:29
+    Autogenerated on: 2023-04-18
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class DiseasePanel(_ParentRestClient):
     """
     This class contains methods for the 'Disease Panels' webservices
-    Client version: 2.6.0-SNAPSHOT [cd4c96caf1cb7afcdec5f54a7de72bde4f63820e]
+    Client version: 2.8.0-SNAPSHOT
     PATH: /{apiVersion}/panels
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(DiseasePanel, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
```

### Comparing `pyopencga-2.7.1/pyopencga/rest_clients/family_client.py` & `pyopencga-2.8.0/pyopencga/rest_clients/family_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-01-10 10:57:29
+    Autogenerated on: 2023-04-18
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Family(_ParentRestClient):
     """
     This class contains methods for the 'Families' webservices
-    Client version: 2.6.0-SNAPSHOT [cd4c96caf1cb7afcdec5f54a7de72bde4f63820e]
+    Client version: 2.8.0-SNAPSHOT
     PATH: /{apiVersion}/families
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Family, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
@@ -267,14 +267,15 @@
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param str study: Study [[user@]project:]study where study and project
             can be either the ID or UUID.
         :param bool update_roles: Update the member roles within the family.
+        :param bool update_pedigree_graph: Update the family pedigree graph.
         :param str annotation_sets_action: Action to be performed if the array
             of annotationSets is being updated. Allowed values: ['ADD SET
             REMOVE']
         :param bool include_result: Flag indicating to include the created or
             updated document result in the response.
         :param dict data: body.
         """
```

### Comparing `pyopencga-2.7.1/pyopencga/rest_clients/file_client.py` & `pyopencga-2.8.0/pyopencga/rest_clients/file_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-01-10 10:57:29
+    Autogenerated on: 2023-04-18
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class File(_ParentRestClient):
     """
     This class contains methods for the 'Files' webservices
-    Client version: 2.6.0-SNAPSHOT [cd4c96caf1cb7afcdec5f54a7de72bde4f63820e]
+    Client version: 2.8.0-SNAPSHOT
     PATH: /{apiVersion}/files
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(File, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
@@ -315,15 +315,15 @@
 
     def upload(self, **options):
         """
         Resource to upload a file by chunks.
         PATH: /{apiVersion}/files/upload
 
         :param inputstream file: File to upload.
-        :param str filename: File name to overwrite the input fileName.
+        :param str file_name: File name to overwrite the input fileName.
         :param str file_format: File format. Allowed values: ['VCF BCF GVCF
             TBI BIGWIG SAM BAM BAI CRAM CRAI FASTQ FASTA PED
             TAB_SEPARATED_VALUES COMMA_SEPARATED_VALUES XML PROTOCOL_BUFFER
             JSON AVRO PARQUET IMAGE PLAIN BINARY NONE UNKNOWN']
         :param str bioformat: File bioformat. Allowed values:
             ['MICROARRAY_EXPRESSION_ONECHANNEL_AGILENT
             MICROARRAY_EXPRESSION_ONECHANNEL_AFFYMETRIX
```

### Comparing `pyopencga-2.7.1/pyopencga/rest_clients/ga4gh_client.py` & `pyopencga-2.8.0/pyopencga/rest_clients/ga4gh_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-01-10 10:57:29
+    Autogenerated on: 2023-04-18
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class GA4GH(_ParentRestClient):
     """
     This class contains methods for the 'GA4GH' webservices
-    Client version: 2.6.0-SNAPSHOT [cd4c96caf1cb7afcdec5f54a7de72bde4f63820e]
+    Client version: 2.8.0-SNAPSHOT
     PATH: /{apiVersion}/ga4gh
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(GA4GH, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def search_reads(self, **options):
```

### Comparing `pyopencga-2.7.1/pyopencga/rest_clients/individual_client.py` & `pyopencga-2.8.0/pyopencga/rest_clients/individual_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-01-10 10:57:29
+    Autogenerated on: 2023-04-18
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Individual(_ParentRestClient):
     """
     This class contains methods for the 'Individuals' webservices
-    Client version: 2.6.0-SNAPSHOT [cd4c96caf1cb7afcdec5f54a7de72bde4f63820e]
+    Client version: 2.8.0-SNAPSHOT
     PATH: /{apiVersion}/individuals
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Individual, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
```

### Comparing `pyopencga-2.7.1/pyopencga/rest_clients/job_client.py` & `pyopencga-2.8.0/pyopencga/rest_clients/job_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-01-10 10:57:29
+    Autogenerated on: 2023-04-18
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Job(_ParentRestClient):
     """
     This class contains methods for the 'Jobs' webservices
-    Client version: 2.6.0-SNAPSHOT [cd4c96caf1cb7afcdec5f54a7de72bde4f63820e]
+    Client version: 2.8.0-SNAPSHOT
     PATH: /{apiVersion}/jobs
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Job, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
```

### Comparing `pyopencga-2.7.1/pyopencga/rest_clients/meta_client.py` & `pyopencga-2.8.0/pyopencga/rest_clients/meta_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-01-10 10:57:29
+    Autogenerated on: 2023-04-18
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Meta(_ParentRestClient):
     """
     This class contains methods for the 'Meta' webservices
-    Client version: 2.6.0-SNAPSHOT [cd4c96caf1cb7afcdec5f54a7de72bde4f63820e]
+    Client version: 2.8.0-SNAPSHOT
     PATH: /{apiVersion}/meta
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Meta, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def about(self, **options):
```

### Comparing `pyopencga-2.7.1/pyopencga/rest_clients/project_client.py` & `pyopencga-2.8.0/pyopencga/rest_clients/project_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-01-10 10:57:29
+    Autogenerated on: 2023-04-18
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Project(_ParentRestClient):
     """
     This class contains methods for the 'Projects' webservices
-    Client version: 2.6.0-SNAPSHOT [cd4c96caf1cb7afcdec5f54a7de72bde4f63820e]
+    Client version: 2.8.0-SNAPSHOT
     PATH: /{apiVersion}/projects
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Project, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def create(self, data=None, **options):
```

### Comparing `pyopencga-2.7.1/pyopencga/rest_clients/sample_client.py` & `pyopencga-2.8.0/pyopencga/rest_clients/sample_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-01-10 10:57:29
+    Autogenerated on: 2023-04-18
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Sample(_ParentRestClient):
     """
     This class contains methods for the 'Samples' webservices
-    Client version: 2.6.0-SNAPSHOT [cd4c96caf1cb7afcdec5f54a7de72bde4f63820e]
+    Client version: 2.8.0-SNAPSHOT
     PATH: /{apiVersion}/samples
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Sample, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
```

### Comparing `pyopencga-2.7.1/pyopencga/rest_clients/study_client.py` & `pyopencga-2.8.0/pyopencga/rest_clients/study_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-01-10 10:57:29
+    Autogenerated on: 2023-04-18
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Study(_ParentRestClient):
     """
     This class contains methods for the 'Studies' webservices
-    Client version: 2.6.0-SNAPSHOT [cd4c96caf1cb7afcdec5f54a7de72bde4f63820e]
+    Client version: 2.8.0-SNAPSHOT
     PATH: /{apiVersion}/studies
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Study, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
```

### Comparing `pyopencga-2.7.1/pyopencga/rest_clients/user_client.py` & `pyopencga-2.8.0/pyopencga/rest_clients/user_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,30 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-01-10 10:57:29
+    Autogenerated on: 2023-04-18
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class User(_ParentRestClient):
     """
     This class contains methods for the 'Users' webservices
-    Client version: 2.6.0-SNAPSHOT [cd4c96caf1cb7afcdec5f54a7de72bde4f63820e]
+    Client version: 2.8.0-SNAPSHOT
     PATH: /{apiVersion}/users
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(User, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
-    def create(self, data=None, **options):
-        """
-        Create a new user.
-        PATH: /{apiVersion}/users/create
-
-        :param dict data: JSON containing the parameters. (REQUIRED)
-        """
-
-        return self._post(category='users', resource='create', data=data, **options)
-
     def login(self, data=None, **options):
         """
         Get identified and gain access to the system.
         PATH: /{apiVersion}/users/login
 
         :param dict data: JSON containing the authentication parameters.
         """
```

### Comparing `pyopencga-2.7.1/pyopencga/rest_clients/variant_client.py` & `pyopencga-2.8.0/pyopencga/rest_clients/variant_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-01-10 10:57:29
+    Autogenerated on: 2023-04-18
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Variant(_ParentRestClient):
     """
     This class contains methods for the 'Analysis - Variant' webservices
-    Client version: 2.6.0-SNAPSHOT [cd4c96caf1cb7afcdec5f54a7de72bde4f63820e]
+    Client version: 2.8.0-SNAPSHOT
     PATH: /{apiVersion}/analysis/variant
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Variant, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def aggregation_stats(self, **options):
```

### Comparing `pyopencga-2.7.1/pyopencga/rest_clients/variant_operation_client.py` & `pyopencga-2.8.0/pyopencga/rest_clients/variant_operation_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-01-10 10:57:29
+    Autogenerated on: 2023-04-18
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class VariantOperation(_ParentRestClient):
     """
     This class contains methods for the 'Operations - Variant Storage' webservices
-    Client version: 2.6.0-SNAPSHOT [cd4c96caf1cb7afcdec5f54a7de72bde4f63820e]
+    Client version: 2.8.0-SNAPSHOT
     PATH: /{apiVersion}/operation
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(VariantOperation, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def configure_cellbase(self, data=None, **options):
@@ -403,15 +403,15 @@
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         :param str project: Project [user@]project where project can be either
             the ID or the alias.
         :param str study: Study [[user@]project:]study where study and project
             can be either the ID or UUID.
-        :param dict data: Variant secondary index params.
+        :param dict data: Variant secondary annotation index params.
         """
 
         return self._post(category='operation', resource='index', subcategory='variant/secondary/annotation', data=data, **options)
 
     def variant_secondary_sample_index(self, data=None, **options):
         """
         Build and annotate the sample index. (New!) .
@@ -454,15 +454,15 @@
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         :param str project: Project [user@]project where project can be either
             the ID or the alias.
         :param str study: Study [[user@]project:]study where study and project
             can be either the ID or UUID.
-        :param dict data: Variant secondary index params.
+        :param dict data: Variant secondary annotation index params.
         """
 
         return self._post(category='operation', resource='secondaryIndex', subcategory='variant', data=data, **options)
 
     def delete_variant_secondary_index(self, **options):
         """
         Remove a secondary index from the search engine for a specific set of
```

### Comparing `pyopencga-2.7.1/pyopencga/rest_response.py` & `pyopencga-2.8.0/pyopencga/rest_response.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.7.1/pyopencga/retry.py` & `pyopencga-2.8.0/pyopencga/retry.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.7.1/pyopencga.egg-info/PKG-INFO` & `pyopencga-2.8.0/pyopencga.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencga
-Version: 2.7.1
+Version: 2.8.0
 Summary: A REST client for OpenCGA REST web services
 Home-page: https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga
 Author: David Gomez-Peregrina, Pablo Marin-Garcia, Daniel Perez-Gil
 Author-email: david.gomez@mgviz.org, pmarin@kanteron.com, dp529@cam.ac.uk
 License: Apache Software License
 Project-URL: Documentation, http://docs.opencb.org/display/opencga/Python
 Project-URL: Source, https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga
```

### Comparing `pyopencga-2.7.1/pyopencga.egg-info/SOURCES.txt` & `pyopencga-2.8.0/pyopencga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyopencga-2.7.1/setup.py` & `pyopencga-2.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pyopencga',
-    version='2.7.1',
+    version='2.8.0',
     description='A REST client for OpenCGA REST web services',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     url='https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga',
     packages=['pyopencga', 'pyopencga.rest_clients'],
     license='Apache Software License',
     author='David Gomez-Peregrina, Pablo Marin-Garcia, Daniel Perez-Gil',
```

