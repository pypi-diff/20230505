# Comparing `tmp/v7e_utils-0.2.0.tar.gz` & `tmp/v7e_utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "v7e_utils-0.2.0.tar", max compression
+gzip compressed data, was "v7e_utils-0.3.0.tar", max compression
```

## Comparing `v7e_utils-0.2.0.tar` & `v7e_utils-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      483 2023-05-02 18:29:43.648755 v7e_utils-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-26 20:54:37.830739 v7e_utils-0.2.0/v7e_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 20:54:37.830739 v7e_utils-0.2.0/v7e_utils/agil_connect/__init__.py
--rw-r--r--   0        0        0     1207 2023-04-26 20:54:37.830739 v7e_utils-0.2.0/v7e_utils/agil_connect/agil_connect.py
--rw-r--r--   0        0        0     1251 2023-05-02 18:30:45.743777 v7e_utils-0.2.0/v7e_utils/agil_connect/panel_connect.py
--rw-r--r--   0        0        0     1890 2023-05-02 18:30:45.743777 v7e_utils-0.2.0/v7e_utils/agil_connect/rh_connect.py
--rw-r--r--   0        0        0       67 2023-04-26 20:54:37.830739 v7e_utils-0.2.0/v7e_utils/data_helper/__init__.py
--rw-r--r--   0        0        0    10801 2023-05-02 18:30:45.747778 v7e_utils-0.2.0/v7e_utils/data_helper/data_helper.py
--rw-r--r--   0        0        0      813 2023-04-26 20:54:37.830739 v7e_utils-0.2.0/v7e_utils/data_helper/error.py
--rw-r--r--   0        0        0     1015 2023-04-26 20:54:37.830739 v7e_utils-0.2.0/v7e_utils/data_helper/record_batch.py
--rw-r--r--   0        0        0     3081 2023-04-26 20:54:37.830739 v7e_utils-0.2.0/v7e_utils/data_utils.py
--rw-r--r--   0        0        0       65 2023-04-26 20:54:37.830739 v7e_utils-0.2.0/v7e_utils/dataframe_helper/__init__.py
--rw-r--r--   0        0        0     6891 2023-04-26 20:54:37.830739 v7e_utils-0.2.0/v7e_utils/dataframe_helper/df_helper.py
--rw-r--r--   0        0        0     5854 2023-04-26 20:54:37.830739 v7e_utils-0.2.0/v7e_utils/dataframe_helper/io.py
--rw-r--r--   0        0        0     3053 2023-04-26 20:54:37.830739 v7e_utils-0.2.0/v7e_utils/dataframe_helper/utils.py
--rw-r--r--   0        0        0     7836 2023-04-26 20:54:37.830739 v7e_utils-0.2.0/v7e_utils/date_utils.py
--rw-r--r--   0        0        0     3676 2023-04-26 20:54:37.830739 v7e_utils-0.2.0/v7e_utils/file_utils.py
--rw-r--r--   0        0        0      577 2023-04-26 20:54:37.830739 v7e_utils-0.2.0/v7e_utils/model_utils.py
--rw-r--r--   0        0        0       65 2023-04-26 20:54:37.830739 v7e_utils-0.2.0/v7e_utils/report_factory/__init__.py
--rw-r--r--   0        0        0      815 2023-04-26 20:54:37.830739 v7e_utils-0.2.0/v7e_utils/report_factory/factory.py
--rw-r--r--   0        0        0      494 2023-04-26 20:54:37.830739 v7e_utils-0.2.0/v7e_utils/report_factory/loader.py
--rw-r--r--   0        0        0     4217 2023-05-02 18:30:45.747778 v7e_utils-0.2.0/v7e_utils/report_factory/publisher.py
--rw-r--r--   0        0        0     1245 2023-04-26 20:54:37.830739 v7e_utils-0.2.0/v7e_utils/report_factory/report_helper.py
--rw-r--r--   0        0        0      508 2023-04-26 20:54:37.830739 v7e_utils-0.2.0/v7e_utils/report_factory/reporter.py
--rw-r--r--   0        0        0      387 2023-04-26 20:54:37.830739 v7e_utils-0.2.0/v7e_utils/report_factory/runner.py
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 v7e_utils-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      457 2023-05-05 19:58:14.788928 v7e_utils-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-26 20:54:37.830739 v7e_utils-0.3.0/v7e_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 20:54:37.830739 v7e_utils-0.3.0/v7e_utils/agil_connect/__init__.py
+-rw-r--r--   0        0        0     1207 2023-04-26 20:54:37.830739 v7e_utils-0.3.0/v7e_utils/agil_connect/agil_connect.py
+-rw-r--r--   0        0        0     1251 2023-05-02 18:30:45.743777 v7e_utils-0.3.0/v7e_utils/agil_connect/panel_connect.py
+-rw-r--r--   0        0        0     2227 2023-05-05 19:56:30.535853 v7e_utils-0.3.0/v7e_utils/agil_connect/rh_connect.py
+-rw-r--r--   0        0        0       67 2023-04-26 20:54:37.830739 v7e_utils-0.3.0/v7e_utils/data_helper/__init__.py
+-rw-r--r--   0        0        0    10801 2023-05-02 18:30:45.747778 v7e_utils-0.3.0/v7e_utils/data_helper/data_helper.py
+-rw-r--r--   0        0        0      813 2023-04-26 20:54:37.830739 v7e_utils-0.3.0/v7e_utils/data_helper/error.py
+-rw-r--r--   0        0        0     1015 2023-04-26 20:54:37.830739 v7e_utils-0.3.0/v7e_utils/data_helper/record_batch.py
+-rw-r--r--   0        0        0     3081 2023-04-26 20:54:37.830739 v7e_utils-0.3.0/v7e_utils/data_utils.py
+-rw-r--r--   0        0        0       65 2023-04-26 20:54:37.830739 v7e_utils-0.3.0/v7e_utils/dataframe_helper/__init__.py
+-rw-r--r--   0        0        0     6891 2023-04-26 20:54:37.830739 v7e_utils-0.3.0/v7e_utils/dataframe_helper/df_helper.py
+-rw-r--r--   0        0        0     5854 2023-04-26 20:54:37.830739 v7e_utils-0.3.0/v7e_utils/dataframe_helper/io.py
+-rw-r--r--   0        0        0     3053 2023-04-26 20:54:37.830739 v7e_utils-0.3.0/v7e_utils/dataframe_helper/utils.py
+-rw-r--r--   0        0        0     7836 2023-04-26 20:54:37.830739 v7e_utils-0.3.0/v7e_utils/date_utils.py
+-rw-r--r--   0        0        0     3676 2023-04-26 20:54:37.830739 v7e_utils-0.3.0/v7e_utils/file_utils.py
+-rw-r--r--   0        0        0      577 2023-04-26 20:54:37.830739 v7e_utils-0.3.0/v7e_utils/model_utils.py
+-rw-r--r--   0        0        0       65 2023-04-26 20:54:37.830739 v7e_utils-0.3.0/v7e_utils/report_factory/__init__.py
+-rw-r--r--   0        0        0      815 2023-04-26 20:54:37.830739 v7e_utils-0.3.0/v7e_utils/report_factory/factory.py
+-rw-r--r--   0        0        0      494 2023-04-26 20:54:37.830739 v7e_utils-0.3.0/v7e_utils/report_factory/loader.py
+-rw-r--r--   0        0        0     4217 2023-05-02 18:30:45.747778 v7e_utils-0.3.0/v7e_utils/report_factory/publisher.py
+-rw-r--r--   0        0        0     1245 2023-04-26 20:54:37.830739 v7e_utils-0.3.0/v7e_utils/report_factory/report_helper.py
+-rw-r--r--   0        0        0      508 2023-04-26 20:54:37.830739 v7e_utils-0.3.0/v7e_utils/report_factory/reporter.py
+-rw-r--r--   0        0        0      387 2023-04-26 20:54:37.830739 v7e_utils-0.3.0/v7e_utils/report_factory/runner.py
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 v7e_utils-0.3.0/PKG-INFO
```

### Comparing `v7e_utils-0.2.0/v7e_utils/agil_connect/agil_connect.py` & `v7e_utils-0.3.0/v7e_utils/agil_connect/agil_connect.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.2.0/v7e_utils/agil_connect/panel_connect.py` & `v7e_utils-0.3.0/v7e_utils/agil_connect/panel_connect.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.2.0/v7e_utils/agil_connect/rh_connect.py` & `v7e_utils-0.3.0/v7e_utils/agil_connect/rh_connect.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 from v7e_utils.agil_connect.agil_connect import AgilConnection
 from urllib.parse import urlencode
 
+class RhSingleEmployee(AgilConnection):
+    def __init__(self, url=None):
+        super().__init__(url)
+        self.set_api_endpoint('paf/employeeBasicInfo/')
+
+    def get_rh_employees_single(self, parameters):
+        url = self.ensure_url(self.gateway_url, self.api_endpoint)
+        return self.get_result(url, parameters)
+    
+    
 class RhEmployees(AgilConnection):
     def __init__(self, url=None):
         super().__init__(url)
         self.set_api_endpoint('paf/allEmployeesBasicInfo/')
 
     def get_rh_employees_single(self, person):
         url = self.ensure_url(self.gateway_url, self.api_endpoint)
```

### Comparing `v7e_utils-0.2.0/v7e_utils/data_helper/data_helper.py` & `v7e_utils-0.3.0/v7e_utils/data_helper/data_helper.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.2.0/v7e_utils/data_helper/error.py` & `v7e_utils-0.3.0/v7e_utils/data_helper/error.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.2.0/v7e_utils/data_helper/record_batch.py` & `v7e_utils-0.3.0/v7e_utils/data_helper/record_batch.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.2.0/v7e_utils/data_utils.py` & `v7e_utils-0.3.0/v7e_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.2.0/v7e_utils/dataframe_helper/df_helper.py` & `v7e_utils-0.3.0/v7e_utils/dataframe_helper/df_helper.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.2.0/v7e_utils/dataframe_helper/io.py` & `v7e_utils-0.3.0/v7e_utils/dataframe_helper/io.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.2.0/v7e_utils/dataframe_helper/utils.py` & `v7e_utils-0.3.0/v7e_utils/dataframe_helper/utils.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.2.0/v7e_utils/date_utils.py` & `v7e_utils-0.3.0/v7e_utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.2.0/v7e_utils/file_utils.py` & `v7e_utils-0.3.0/v7e_utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.2.0/v7e_utils/model_utils.py` & `v7e_utils-0.3.0/v7e_utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.2.0/v7e_utils/report_factory/factory.py` & `v7e_utils-0.3.0/v7e_utils/report_factory/factory.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.2.0/v7e_utils/report_factory/publisher.py` & `v7e_utils-0.3.0/v7e_utils/report_factory/publisher.py`

 * *Files identical despite different names*

### Comparing `v7e_utils-0.2.0/v7e_utils/report_factory/report_helper.py` & `v7e_utils-0.3.0/v7e_utils/report_factory/report_helper.py`

 * *Files identical despite different names*

