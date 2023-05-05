# Comparing `tmp/pyGuardPoint-0.8.9.tar.gz` & `tmp/pyGuardPoint-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGuardPoint-0.8.9.tar", last modified: Wed Apr 26 10:53:51 2023, max compression
+gzip compressed data, was "pyGuardPoint-0.9.0.tar", last modified: Fri May  5 08:30:54 2023, max compression
```

## Comparing `pyGuardPoint-0.8.9.tar` & `pyGuardPoint-0.9.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 10:53:51.456921 pyGuardPoint-0.8.9/
--rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.8.9/LICENSE.txt
--rw-rw-rw-   0        0        0     5739 2023-04-26 10:53:51.456921 pyGuardPoint-0.8.9/PKG-INFO
--rw-rw-rw-   0        0        0     5480 2023-04-14 14:00:11.000000 pyGuardPoint-0.8.9/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-26 10:53:51.446884 pyGuardPoint-0.8.9/pyGuardPoint/
--rw-rw-rw-   0        0        0      266 2023-04-20 12:58:39.000000 pyGuardPoint-0.8.9/pyGuardPoint/__init__.py
--rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.8.9/pyGuardPoint/_guardpoint_areas.py
--rw-rw-rw-   0        0        0    11195 2023-04-20 13:33:25.000000 pyGuardPoint-0.8.9/pyGuardPoint/_guardpoint_cardholders.py
--rw-rw-rw-   0        0        0     1083 2023-04-20 13:02:16.000000 pyGuardPoint-0.8.9/pyGuardPoint/_guardpoint_cardholdertypes.py
--rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.8.9/pyGuardPoint/_guardpoint_cards.py
--rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.8.9/pyGuardPoint/_guardpoint_customizedfields.py
--rw-rw-rw-   0        0        0     1175 2023-03-16 16:56:01.000000 pyGuardPoint-0.8.9/pyGuardPoint/_guardpoint_personaldetails.py
--rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.8.9/pyGuardPoint/_guardpoint_scheduledmags.py
--rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.8.9/pyGuardPoint/_guardpoint_securitygroups.py
--rw-rw-rw-   0        0        0     5586 2023-04-20 11:51:01.000000 pyGuardPoint-0.8.9/pyGuardPoint/_odata_filter.py
--rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.8.9/pyGuardPoint/_str_match_algo.py
--rw-rw-rw-   0        0        0     2474 2023-04-20 13:02:16.000000 pyGuardPoint-0.8.9/pyGuardPoint/guardpoint.py
--rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.8.9/pyGuardPoint/guardpoint_async.py
--rw-rw-rw-   0        0        0     5898 2023-04-26 10:53:15.000000 pyGuardPoint-0.8.9/pyGuardPoint/guardpoint_connection.py
--rw-rw-rw-   0        0        0    17297 2023-04-20 13:31:08.000000 pyGuardPoint-0.8.9/pyGuardPoint/guardpoint_dataclasses.py
--rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.8.9/pyGuardPoint/guardpoint_error.py
--rw-rw-rw-   0        0        0     3012 2023-04-13 12:30:22.000000 pyGuardPoint-0.8.9/pyGuardPoint/guardpoint_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:53:51.455957 pyGuardPoint-0.8.9/pyGuardPoint.egg-info/
--rw-rw-rw-   0        0        0     5739 2023-04-26 10:53:51.000000 pyGuardPoint-0.8.9/pyGuardPoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      861 2023-04-26 10:53:51.000000 pyGuardPoint-0.8.9/pyGuardPoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 10:53:51.000000 pyGuardPoint-0.8.9/pyGuardPoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.8.9/pyGuardPoint.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-04-26 10:53:51.000000 pyGuardPoint-0.8.9/pyGuardPoint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-26 10:53:51.000000 pyGuardPoint-0.8.9/pyGuardPoint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 10:53:51.457920 pyGuardPoint-0.8.9/setup.cfg
--rw-rw-rw-   0        0        0      549 2023-04-26 10:34:13.000000 pyGuardPoint-0.8.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:30:54.456474 pyGuardPoint-0.9.0/
+-rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     5739 2023-05-05 08:30:54.455475 pyGuardPoint-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5480 2023-04-14 14:00:11.000000 pyGuardPoint-0.9.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-05 08:30:54.445474 pyGuardPoint-0.9.0/pyGuardPoint/
+-rw-rw-rw-   0        0        0      266 2023-04-20 12:58:39.000000 pyGuardPoint-0.9.0/pyGuardPoint/__init__.py
+-rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.9.0/pyGuardPoint/_guardpoint_areas.py
+-rw-rw-rw-   0        0        0    11195 2023-04-20 13:33:25.000000 pyGuardPoint-0.9.0/pyGuardPoint/_guardpoint_cardholders.py
+-rw-rw-rw-   0        0        0     1083 2023-04-20 13:02:16.000000 pyGuardPoint-0.9.0/pyGuardPoint/_guardpoint_cardholdertypes.py
+-rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.9.0/pyGuardPoint/_guardpoint_cards.py
+-rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.9.0/pyGuardPoint/_guardpoint_customizedfields.py
+-rw-rw-rw-   0        0        0     1175 2023-03-16 16:56:01.000000 pyGuardPoint-0.9.0/pyGuardPoint/_guardpoint_personaldetails.py
+-rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.9.0/pyGuardPoint/_guardpoint_scheduledmags.py
+-rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.9.0/pyGuardPoint/_guardpoint_securitygroups.py
+-rw-rw-rw-   0        0        0     5586 2023-04-20 11:51:01.000000 pyGuardPoint-0.9.0/pyGuardPoint/_odata_filter.py
+-rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.9.0/pyGuardPoint/_str_match_algo.py
+-rw-rw-rw-   0        0        0     2474 2023-04-20 13:02:16.000000 pyGuardPoint-0.9.0/pyGuardPoint/guardpoint.py
+-rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.9.0/pyGuardPoint/guardpoint_async.py
+-rw-rw-rw-   0        0        0     5898 2023-04-26 10:53:15.000000 pyGuardPoint-0.9.0/pyGuardPoint/guardpoint_connection.py
+-rw-rw-rw-   0        0        0    17297 2023-04-20 13:31:08.000000 pyGuardPoint-0.9.0/pyGuardPoint/guardpoint_dataclasses.py
+-rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.9.0/pyGuardPoint/guardpoint_error.py
+-rw-rw-rw-   0        0        0     3140 2023-05-04 10:22:18.000000 pyGuardPoint-0.9.0/pyGuardPoint/guardpoint_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:30:54.454479 pyGuardPoint-0.9.0/pyGuardPoint.egg-info/
+-rw-rw-rw-   0        0        0     5739 2023-05-05 08:30:54.000000 pyGuardPoint-0.9.0/pyGuardPoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2023-05-05 08:30:54.000000 pyGuardPoint-0.9.0/pyGuardPoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 08:30:54.000000 pyGuardPoint-0.9.0/pyGuardPoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.9.0/pyGuardPoint.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-05-05 08:30:54.000000 pyGuardPoint-0.9.0/pyGuardPoint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-05 08:30:54.000000 pyGuardPoint-0.9.0/pyGuardPoint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 08:30:54.456474 pyGuardPoint-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      549 2023-05-05 08:30:14.000000 pyGuardPoint-0.9.0/setup.py
```

### Comparing `pyGuardPoint-0.8.9/LICENSE.txt` & `pyGuardPoint-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.9/PKG-INFO` & `pyGuardPoint-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 0.8.9
+Version: 0.9.0
 Summary: Python wrapper for GuardPoint 10 Access Control System
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 pyGuardPoint
```

### Comparing `pyGuardPoint-0.8.9/README.rst` & `pyGuardPoint-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.9/pyGuardPoint/_guardpoint_areas.py` & `pyGuardPoint-0.9.0/pyGuardPoint/_guardpoint_areas.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.9/pyGuardPoint/_guardpoint_cardholders.py` & `pyGuardPoint-0.9.0/pyGuardPoint/_guardpoint_cardholders.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.9/pyGuardPoint/_guardpoint_cardholdertypes.py` & `pyGuardPoint-0.9.0/pyGuardPoint/_guardpoint_cardholdertypes.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.9/pyGuardPoint/_guardpoint_cards.py` & `pyGuardPoint-0.9.0/pyGuardPoint/_guardpoint_cards.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.9/pyGuardPoint/_guardpoint_customizedfields.py` & `pyGuardPoint-0.9.0/pyGuardPoint/_guardpoint_customizedfields.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.9/pyGuardPoint/_guardpoint_personaldetails.py` & `pyGuardPoint-0.9.0/pyGuardPoint/_guardpoint_personaldetails.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.9/pyGuardPoint/_guardpoint_scheduledmags.py` & `pyGuardPoint-0.9.0/pyGuardPoint/_guardpoint_scheduledmags.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.9/pyGuardPoint/_guardpoint_securitygroups.py` & `pyGuardPoint-0.9.0/pyGuardPoint/_guardpoint_securitygroups.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.9/pyGuardPoint/_odata_filter.py` & `pyGuardPoint-0.9.0/pyGuardPoint/_odata_filter.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.9/pyGuardPoint/_str_match_algo.py` & `pyGuardPoint-0.9.0/pyGuardPoint/_str_match_algo.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.9/pyGuardPoint/guardpoint.py` & `pyGuardPoint-0.9.0/pyGuardPoint/guardpoint.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.9/pyGuardPoint/guardpoint_async.py` & `pyGuardPoint-0.9.0/pyGuardPoint/guardpoint_async.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.9/pyGuardPoint/guardpoint_connection.py` & `pyGuardPoint-0.9.0/pyGuardPoint/guardpoint_connection.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.9/pyGuardPoint/guardpoint_dataclasses.py` & `pyGuardPoint-0.9.0/pyGuardPoint/guardpoint_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.9/pyGuardPoint/guardpoint_utils.py` & `pyGuardPoint-0.9.0/pyGuardPoint/guardpoint_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,18 @@
 
 class GuardPointResponse:
     @staticmethod
     def check_odata_body_structure(response_body):
         if not isinstance(response_body, dict):
             raise GuardPointError("Non-JSON Response Body")
         if '@odata.context' not in response_body:
-            raise GuardPointError("Non-ODATA Response Body")
+            if 'error' in response_body:
+                raise GuardPointError(response_body['error'])
+            else:
+                raise GuardPointError("Non-ODATA Response Body")
         if not str(response_body['@odata.context']).endswith("$entity"):
             # Non entities seem to always appear to contain 'value'
             check = False
             for item in response_body:
                 if item in ['value', 'errorMessages', 'message', 'error']:
                     check = True
             if not check:
```

### Comparing `pyGuardPoint-0.8.9/pyGuardPoint.egg-info/PKG-INFO` & `pyGuardPoint-0.9.0/pyGuardPoint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 0.8.9
+Version: 0.9.0
 Summary: Python wrapper for GuardPoint 10 Access Control System
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 pyGuardPoint
```

### Comparing `pyGuardPoint-0.8.9/pyGuardPoint.egg-info/SOURCES.txt` & `pyGuardPoint-0.9.0/pyGuardPoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.9/setup.py` & `pyGuardPoint-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 long_description = open('README.rst').read()
 
 setup(name="pyGuardPoint",
-      version="0.8.9",
+      version="0.9.0",
       author="John Owen",
       description="Python wrapper for GuardPoint 10 Access Control System",
       long_description_content_type='text/markdown',
       long_description=long_description,
       maintainer_email="sales@sensoraccess.co.uk",
       install_requires=['validators', 'fuzzywuzzy', 'Levenshtein'],
       packages=['pyGuardPoint'],
```

