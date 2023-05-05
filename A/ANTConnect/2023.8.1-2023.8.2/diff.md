# Comparing `tmp/ANTConnect-2023.8.1.tar.gz` & `tmp/ANTConnect-2023.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ANTConnect-2023.8.1.tar", last modified: Thu Mar  2 14:04:38 2023, max compression
+gzip compressed data, was "dist\ANTConnect-2023.8.2.tar", last modified: Fri May  5 06:48:00 2023, max compression
```

## Comparing `ANTConnect-2023.8.1.tar` & `ANTConnect-2023.8.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-02 14:04:38.604739 ANTConnect-2023.8.1/
-drwxrwxrwx   0        0        0        0 2023-03-02 14:04:38.596282 ANTConnect-2023.8.1/ANTConnect.egg-info/
--rw-rw-rw-   0        0        0     1017 2023-03-02 14:04:38.000000 ANTConnect-2023.8.1/ANTConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-03-02 14:04:38.000000 ANTConnect-2023.8.1/ANTConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-02 14:04:38.000000 ANTConnect-2023.8.1/ANTConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-02 14:04:38.000000 ANTConnect-2023.8.1/ANTConnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-03-02 14:04:38.000000 ANTConnect-2023.8.1/ANTConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2022-12-21 12:12:30.000000 ANTConnect-2023.8.1/LICENSE
--rw-rw-rw-   0        0        0     1017 2023-03-02 14:04:38.604739 ANTConnect-2023.8.1/PKG-INFO
--rw-rw-rw-   0        0        0      586 2022-12-21 12:12:30.000000 ANTConnect-2023.8.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-02 14:04:38.598708 ANTConnect-2023.8.1/antconnect/
--rw-rw-rw-   0        0        0      146 2023-03-02 14:03:55.000000 ANTConnect-2023.8.1/antconnect/__init__.py
--rw-rw-rw-   0        0        0    50585 2023-03-02 13:56:09.000000 ANTConnect-2023.8.1/antconnect/api.py
--rw-rw-rw-   0        0        0      485 2023-03-02 14:04:38.606734 ANTConnect-2023.8.1/setup.cfg
--rw-rw-rw-   0        0        0      739 2023-03-02 14:03:55.000000 ANTConnect-2023.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-02 14:04:38.603741 ANTConnect-2023.8.1/tests/
--rw-rw-rw-   0        0        0        0 2022-12-21 12:12:30.000000 ANTConnect-2023.8.1/tests/__init__.py
--rw-rw-rw-   0        0        0      102 2022-12-21 12:12:30.000000 ANTConnect-2023.8.1/tests/test_ant.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:48:00.842904 ANTConnect-2023.8.2/
+drwxrwxrwx   0        0        0        0 2023-05-05 06:48:00.836440 ANTConnect-2023.8.2/ANTConnect.egg-info/
+-rw-rw-rw-   0        0        0     1274 2023-05-05 06:48:00.000000 ANTConnect-2023.8.2/ANTConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-05-05 06:48:00.000000 ANTConnect-2023.8.2/ANTConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 06:48:00.000000 ANTConnect-2023.8.2/ANTConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 06:48:00.000000 ANTConnect-2023.8.2/ANTConnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-05 06:48:00.000000 ANTConnect-2023.8.2/ANTConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1274 2023-05-05 06:48:00.842904 ANTConnect-2023.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2021-06-28 09:19:30.000000 ANTConnect-2023.8.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 06:48:00.838403 ANTConnect-2023.8.2/antconnect/
+-rw-rw-rw-   0        0        0      146 2023-05-05 06:47:15.000000 ANTConnect-2023.8.2/antconnect/__init__.py
+-rw-rw-rw-   0        0        0    50894 2023-05-05 06:47:15.000000 ANTConnect-2023.8.2/antconnect/api.py
+-rw-rw-rw-   0        0        0      485 2023-05-05 06:48:00.844901 ANTConnect-2023.8.2/setup.cfg
+-rw-rw-rw-   0        0        0      739 2023-05-05 06:47:15.000000 ANTConnect-2023.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:48:00.841907 ANTConnect-2023.8.2/tests/
+-rw-rw-rw-   0        0        0        0 2020-12-10 14:04:13.000000 ANTConnect-2023.8.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      102 2020-12-10 14:04:13.000000 ANTConnect-2023.8.2/tests/test_ant.py
```

### Comparing `ANTConnect-2023.8.1/ANTConnect.egg-info/PKG-INFO` & `ANTConnect-2023.8.2/ANTConnect.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: ANTConnect
-Version: 2023.8.1
+Version: 2023.8.2
 Summary: Python SDK for ANT Common Data Engineering
 Home-page: https://antcde.io
 Author: ANT CDE
 Author-email: info@antcde.io
+License: UNKNOWN
+Description: # ANTConnect
+        
+        Provides access to an ANT CDE
+        For more details, visit [docs.antcde.io](https://docs.antcde.io/)
+        
+        ## Release notes
+        
+        ### Version 2021.05.1
+        - Updates Tasks API Calls and includes download files
+        
+        ### Version 2021.04
+        - Adds Tasks API calls to the SDK
+        
+        ### Version 2020.20.5
+        - Adds multiple options in column create and column update
+        
+        ### Version 2020.20.2
+        - Complements update of API on ANTCDE
+        
+        ### Version 2020.18.1
+        - Added more consistancy
+        
+        ### Version 0.1.3
+        - Bugfix
+        
+        ### Version 0.1.2
+        - Bugfix Column Create
+        
+        ### Version 0.1.0
+        - Initial version
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ANTConnect
-
-Provides access to an ANT CDE
-For more details, visit [docs.antcde.io](https://docs.antcde.io/)
-
-## Release notes
-
-### Version 2021.05.1
-- Updates Tasks API Calls and includes download files
-
-### Version 2021.04
-- Adds Tasks API calls to the SDK
-
-### Version 2020.20.5
-- Adds multiple options in column create and column update
-
-### Version 2020.20.2
-- Complements update of API on ANTCDE
-
-### Version 2020.18.1
-- Added more consistancy
-
-### Version 0.1.3
-- Bugfix
-
-### Version 0.1.2
-- Bugfix Column Create
-
-### Version 0.1.0
-- Initial version
```

### Comparing `ANTConnect-2023.8.1/PKG-INFO` & `ANTConnect-2023.8.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: ANTConnect
-Version: 2023.8.1
+Version: 2023.8.2
 Summary: Python SDK for ANT Common Data Engineering
 Home-page: https://antcde.io
 Author: ANT CDE
 Author-email: info@antcde.io
+License: UNKNOWN
+Description: # ANTConnect
+        
+        Provides access to an ANT CDE
+        For more details, visit [docs.antcde.io](https://docs.antcde.io/)
+        
+        ## Release notes
+        
+        ### Version 2021.05.1
+        - Updates Tasks API Calls and includes download files
+        
+        ### Version 2021.04
+        - Adds Tasks API calls to the SDK
+        
+        ### Version 2020.20.5
+        - Adds multiple options in column create and column update
+        
+        ### Version 2020.20.2
+        - Complements update of API on ANTCDE
+        
+        ### Version 2020.18.1
+        - Added more consistancy
+        
+        ### Version 0.1.3
+        - Bugfix
+        
+        ### Version 0.1.2
+        - Bugfix Column Create
+        
+        ### Version 0.1.0
+        - Initial version
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ANTConnect
-
-Provides access to an ANT CDE
-For more details, visit [docs.antcde.io](https://docs.antcde.io/)
-
-## Release notes
-
-### Version 2021.05.1
-- Updates Tasks API Calls and includes download files
-
-### Version 2021.04
-- Adds Tasks API calls to the SDK
-
-### Version 2020.20.5
-- Adds multiple options in column create and column update
-
-### Version 2020.20.2
-- Complements update of API on ANTCDE
-
-### Version 2020.18.1
-- Added more consistancy
-
-### Version 0.1.3
-- Bugfix
-
-### Version 0.1.2
-- Bugfix Column Create
-
-### Version 0.1.0
-- Initial version
```

### Comparing `ANTConnect-2023.8.1/README.md` & `ANTConnect-2023.8.2/README.md`

 * *Files identical despite different names*

### Comparing `ANTConnect-2023.8.1/antconnect/api.py` & `ANTConnect-2023.8.2/antconnect/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -855,14 +855,24 @@
             depreciationMessage("param", "due_date", "01-03-2023", "taken")
             self.update_task(due_date=due_date)
         if appendix != {}:
             depreciationMessage("param", "due_date", "01-03-2023", "taken")
 
         return self._make_api_request(path, 'POST', {"message": response})
 
+    def task_close(self, task_id: str):
+        path = 'tasks/{}/close'.format(task_id)
+
+        return self._make_api_request(path, 'POST')
+
+    def task_cancel(self, task_id: str):
+        path = 'tasks/{}/cancel'.format(task_id)
+
+        return self._make_api_request(path, 'POST')
+
     def update_task(self, task_id: str, title: str = "", description: str = "", priority: str = "",
                     planned_start: str = "", planned_end: str = "", assigned_to: str = "", due_date: str = "",
                     sbs_code: str = "") -> dict:
         """ update a task info"""
         path = "tasks/{}".format(task_id)
         body = {}
         if title != "":
@@ -926,15 +936,15 @@
     def create_virtual_csv(self, records: list):
         """Not for use. Create a virtual CSV of records"""
         encoded_csv = ",".join(records[0].keys()) + "\n"
         for record in records:
             recs = []
             for key in record.keys():
                 recs.append(record[key])
-            encoded_csv += ",".join(recs) + "\n"
+            encoded_csv += "\"" + "\",\"".join(recs) + "\"\n"
         return encoded_csv
 
     def create_virtual_csv_Addid(self, records: list):
         """Not for use. Create a virtual CSV of records"""
         encoded_csv = "id," + ",".join(records[0].keys()) + "\n"
         for record in records:
             recs = []
```

### Comparing `ANTConnect-2023.8.1/setup.py` & `ANTConnect-2023.8.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ANTConnect", # Replace with your own username
-    version="2023.8.1",
+    version="2023.8.2",
     author="ANT CDE",
     author_email="info@antcde.io",
     description="Python SDK for ANT Common Data Engineering",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://antcde.io",
     packages=setuptools.find_packages(),
```

