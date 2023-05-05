# Comparing `tmp/nvcl-kit-1.0.2.tar.gz` & `tmp/nvcl-kit-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvcl-kit-1.0.2.tar", last modified: Tue Mar 21 06:17:35 2023, max compression
+gzip compressed data, was "nvcl-kit-1.1.0.tar", last modified: Fri May  5 06:33:24 2023, max compression
```

## Comparing `nvcl-kit-1.0.2.tar` & `nvcl-kit-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3915 2023-03-21 06:17:08.485111 nvcl-kit-1.0.2/LICENSE
--rw-r--r--   0        0        0     2565 2023-03-21 06:17:08.485111 nvcl-kit-1.0.2/README.md
--rw-r--r--   0        0        0       14 2023-03-21 06:17:08.636122 nvcl-kit-1.0.2/nvcl_kit/__init__.py
--rw-r--r--   0        0        0     5048 2023-03-21 06:17:08.636122 nvcl-kit-1.0.2/nvcl_kit/constants.py
--rw-r--r--   0        0        0     4386 2023-03-21 06:17:08.636122 nvcl-kit-1.0.2/nvcl_kit/generators.py
--rw-r--r--   0        0        0     5379 2023-03-21 06:17:08.636122 nvcl-kit-1.0.2/nvcl_kit/param_builder.py
--rw-r--r--   0        0        0    40275 2023-03-21 06:17:08.637122 nvcl-kit-1.0.2/nvcl_kit/reader.py
--rw-r--r--   0        0        0    14878 2023-03-21 06:17:08.637122 nvcl-kit-1.0.2/nvcl_kit/svc_interface.py
--rw-r--r--   0        0        0    10805 2023-03-21 06:17:08.637122 nvcl-kit-1.0.2/nvcl_kit/wfs_helpers.py
--rw-r--r--   0        0        0      360 2023-03-21 06:17:08.637122 nvcl-kit-1.0.2/nvcl_kit/xml_helpers.py
--rw-r--r--   0        0        0     1039 2023-03-21 06:17:08.637122 nvcl-kit-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3326 1970-01-01 00:00:00.000000 nvcl-kit-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3915 2023-05-05 06:32:59.261547 nvcl-kit-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2823 2023-05-05 06:32:59.261547 nvcl-kit-1.1.0/README.md
+-rw-r--r--   0        0        0       14 2023-05-05 06:32:59.406561 nvcl-kit-1.1.0/nvcl_kit/__init__.py
+-rw-r--r--   0        0        0     5048 2023-05-05 06:32:59.406561 nvcl-kit-1.1.0/nvcl_kit/constants.py
+-rw-r--r--   0        0        0     4386 2023-05-05 06:32:59.406561 nvcl-kit-1.1.0/nvcl_kit/generators.py
+-rw-r--r--   0        0        0     5379 2023-05-05 06:32:59.406561 nvcl-kit-1.1.0/nvcl_kit/param_builder.py
+-rw-r--r--   0        0        0    40851 2023-05-05 06:32:59.406561 nvcl-kit-1.1.0/nvcl_kit/reader.py
+-rw-r--r--   0        0        0    14878 2023-05-05 06:32:59.406561 nvcl-kit-1.1.0/nvcl_kit/svc_interface.py
+-rw-r--r--   0        0        0    10805 2023-05-05 06:32:59.406561 nvcl-kit-1.1.0/nvcl_kit/wfs_helpers.py
+-rw-r--r--   0        0        0      360 2023-05-05 06:32:59.407561 nvcl-kit-1.1.0/nvcl_kit/xml_helpers.py
+-rw-r--r--   0        0        0     1039 2023-05-05 06:32:59.407561 nvcl-kit-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 nvcl-kit-1.1.0/PKG-INFO
```

### Comparing `nvcl-kit-1.0.2/LICENSE` & `nvcl-kit-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.0.2/README.md` & `nvcl-kit-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -28,7 +28,13 @@
 3. There is a rough demonstration script [here](https://gitlab.com/csiro-geoanalytics/python-shared/nvcl_kit/-/blob/master/demo.py)
 4. API documentation can be found [here](https://csiro-geoanalytics.gitlab.io/python-shared/nvcl_kit)
 
 
 ## License
 
 **nvcl_kit** is available under [CSIRO Open Source Software Licence Agreement](LICENSE) (variation of the BSD / MIT License)
+
+## Citation
+
+If you use this package in your research please cite:
+
+Fazio, Vincent; Mule, Shane (2023): nvcl_kit: Access AuScope National Virtual Core Library (NVCL) data services. CSIRO. Service Collection. http://hdl.handle.net/102.100.100/480016?index=1
```

### Comparing `nvcl-kit-1.0.2/nvcl_kit/constants.py` & `nvcl-kit-1.1.0/nvcl_kit/constants.py`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.0.2/nvcl_kit/generators.py` & `nvcl-kit-1.1.0/nvcl_kit/generators.py`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.0.2/nvcl_kit/param_builder.py` & `nvcl-kit-1.1.0/nvcl_kit/param_builder.py`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.0.2/nvcl_kit/reader.py` & `nvcl-kit-1.1.0/nvcl_kit/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -620,32 +620,44 @@
     def get_logs_data(self, nvcl_id):
         ''' Retrieves a set of generic log data for a particular borehole, given an nvcl id
 
         :param nvcl_id: NVCL 'holeidentifier' parameter,
                         the 'nvcl_id' from each item retrieved from 'get_feature_list()' or 'get_nvcl_id_list()'
 
         :returns: a list of SimpleNamespace() objects with attributes:
-                  log_id, log_name, is_public, log_type, algorithm_id, mask_log_id
-                  'mask_log_id' is not supported by all services and may be an empty string'''
+                  log_id, log_name, is_public, log_type, algorithm_id, mask_log_id,
+                     modified_date (optional datetime object not supported by all services)
+                  NB: 'mask_log_id' is not supported by all services and may be an empty string'''
         response_str = self.svc.get_dataset_collection(nvcl_id)
         if not response_str:
             return []
         root = clean_xml_parse(response_str)
         log_list = []
         for ds_child in root.findall('./Dataset'):
+            # Get the modified date
+            date_str = ds_child.findtext('./modifiedDate', default='')
+            date_obj = None
+            if date_str:
+                # Try to parse the modified date from the dataset attributes
+                try:
+                    date_obj = parse(date_str)
+                except ParserError:
+                    pass
             for log_child in ds_child.findall('./Logs/Log'):
                 log_id = log_child.findtext('LogID', default='')
                 log_name = log_child.findtext('logName', default='')
                 is_public = log_child.findtext('ispublic', default='')
                 log_type = log_child.findtext('logType', default='')
                 algorithm_id = log_child.findtext('algorithmoutID', default='')
                 mask_log_id = log_child.findtext('maskLogId', default='')
                 if log_name != '' and log_id != '':
                     log_obj = SimpleNamespace(log_id=log_id, log_name=log_name, is_public=is_public, log_type=log_type,
                                               algorithm_id=algorithm_id, mask_log_id=mask_log_id)
+                    if date_obj is not None:
+                        setattr(log_obj, 'modified_date', date_obj)
                     log_list.append(log_obj)
         return log_list
 
     def get_imagelog_data(self, nvcl_id):
         ''' Retrieves a set of image log data for a particular borehole
 
         :param nvcl_id: NVCL 'holeidentifier' parameter,
```

### Comparing `nvcl-kit-1.0.2/nvcl_kit/svc_interface.py` & `nvcl-kit-1.1.0/nvcl_kit/svc_interface.py`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.0.2/nvcl_kit/wfs_helpers.py` & `nvcl-kit-1.1.0/nvcl_kit/wfs_helpers.py`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.0.2/pyproject.toml` & `nvcl-kit-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "nvcl_kit"
-version = "1.0.2"
+version = "1.1.0"
 description = "Downloads Australian NVCL datasets"
 authors = [
     { name = "Vincent Fazio", email = "vincent.fazio@csiro.au" },
 ]
 dependencies = [
     "owslib==0.28.1",
     "shapely~=2.0",
```

### Comparing `nvcl-kit-1.0.2/PKG-INFO` & `nvcl-kit-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvcl_kit
-Version: 1.0.2
+Version: 1.1.0
 Summary: Downloads Australian NVCL datasets
 License: CSIRO BSD/MIT
 Author-email: Vincent Fazio <vincent.fazio@csiro.au>
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -48,7 +48,13 @@
 4. API documentation can be found [here](https://csiro-geoanalytics.gitlab.io/python-shared/nvcl_kit)
 
 
 ## License
 
 **nvcl_kit** is available under [CSIRO Open Source Software Licence Agreement](LICENSE) (variation of the BSD / MIT License)
 
+## Citation
+
+If you use this package in your research please cite:
+
+Fazio, Vincent; Mule, Shane (2023): nvcl_kit: Access AuScope National Virtual Core Library (NVCL) data services. CSIRO. Service Collection. http://hdl.handle.net/102.100.100/480016?index=1
+
```

