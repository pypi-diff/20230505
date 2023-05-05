# Comparing `tmp/ta_sites-0.4.5.tar.gz` & `tmp/ta_sites-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-kfgtcee9/ta_sites-0.4.5.tar", last modified: Fri Apr 28 11:04:51 2023, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-az6g38pc/ta_sites-0.4.6.tar", last modified: Fri May  5 15:14:01 2023, max compression
```

## Comparing `ta_sites-0.4.5.tar` & `ta_sites-0.4.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 11:04:50.997998 ta_sites-0.4.5/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-28 11:04:30.000000 ta_sites-0.4.5/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-04-28 11:04:30.000000 ta_sites-0.4.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-28 11:04:50.997998 ta_sites-0.4.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      364 2023-04-28 11:04:30.000000 ta_sites-0.4.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-04-28 11:04:50.997998 ta_sites-0.4.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-04-28 11:04:30.000000 ta_sites-0.4.5/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 11:04:50.993998 ta_sites-0.4.5/ta_sites/
--rw-rw-rw-   0 root         (0) root         (0)      602 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 11:04:50.993998 ta_sites-0.4.5/ta_sites/always_care/
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/always_care/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/always_care/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     9569 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/always_care/requests_core.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 11:04:50.997998 ta_sites-0.4.5/ta_sites/basic/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/basic/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4304 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/basic/core.py
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/basic/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 11:04:50.997998 ta_sites-0.4.5/ta_sites/central_reach/
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/central_reach/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17159 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/central_reach/core.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/central_reach/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     9652 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/central_reach/requests_core.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 11:04:50.997998 ta_sites-0.4.5/ta_sites/quickbooks/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/quickbooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25674 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/quickbooks/core.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/quickbooks/grouped_row.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 11:04:50.997998 ta_sites-0.4.5/ta_sites/salesforce/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/salesforce/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2654 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/salesforce/core.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 11:04:50.997998 ta_sites-0.4.5/ta_sites/versant/
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/versant/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/versant/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10568 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/versant/requests_core.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 11:04:50.993998 ta_sites-0.4.5/ta_sites.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-28 11:04:50.000000 ta_sites-0.4.5/ta_sites.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      836 2023-04-28 11:04:50.000000 ta_sites-0.4.5/ta_sites.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-28 11:04:50.000000 ta_sites-0.4.5/ta_sites.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-28 11:04:50.000000 ta_sites-0.4.5/ta_sites.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-28 11:04:50.000000 ta_sites-0.4.5/ta_sites.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-04-28 11:04:50.000000 ta_sites-0.4.5/ta_sites.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 15:14:01.197783 ta_sites-0.4.6/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-05-05 15:13:38.000000 ta_sites-0.4.6/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-05-05 15:13:38.000000 ta_sites-0.4.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-05-05 15:14:01.197783 ta_sites-0.4.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      364 2023-05-05 15:13:38.000000 ta_sites-0.4.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-05-05 15:14:01.197783 ta_sites-0.4.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2023-05-05 15:13:38.000000 ta_sites-0.4.6/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 15:14:01.189783 ta_sites-0.4.6/ta_sites/
+-rw-rw-rw-   0 root         (0) root         (0)      602 2023-05-05 15:13:38.000000 ta_sites-0.4.6/ta_sites/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 15:14:01.193783 ta_sites-0.4.6/ta_sites/always_care/
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-05-05 15:13:38.000000 ta_sites-0.4.6/ta_sites/always_care/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-05-05 15:13:38.000000 ta_sites-0.4.6/ta_sites/always_care/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9569 2023-05-05 15:13:38.000000 ta_sites-0.4.6/ta_sites/always_care/requests_core.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 15:14:01.193783 ta_sites-0.4.6/ta_sites/basic/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 15:13:38.000000 ta_sites-0.4.6/ta_sites/basic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4304 2023-05-05 15:13:38.000000 ta_sites-0.4.6/ta_sites/basic/core.py
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-05-05 15:13:38.000000 ta_sites-0.4.6/ta_sites/basic/exceptions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 15:14:01.193783 ta_sites-0.4.6/ta_sites/central_reach/
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-05-05 15:13:38.000000 ta_sites-0.4.6/ta_sites/central_reach/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17159 2023-05-05 15:13:38.000000 ta_sites-0.4.6/ta_sites/central_reach/core.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2023-05-05 15:13:38.000000 ta_sites-0.4.6/ta_sites/central_reach/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10091 2023-05-05 15:13:38.000000 ta_sites-0.4.6/ta_sites/central_reach/requests_core.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 15:14:01.197783 ta_sites-0.4.6/ta_sites/quickbooks/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-05-05 15:13:38.000000 ta_sites-0.4.6/ta_sites/quickbooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25674 2023-05-05 15:13:38.000000 ta_sites-0.4.6/ta_sites/quickbooks/core.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-05-05 15:13:38.000000 ta_sites-0.4.6/ta_sites/quickbooks/grouped_row.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 15:14:01.197783 ta_sites-0.4.6/ta_sites/salesforce/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-05-05 15:13:38.000000 ta_sites-0.4.6/ta_sites/salesforce/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2654 2023-05-05 15:13:38.000000 ta_sites-0.4.6/ta_sites/salesforce/core.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 15:14:01.197783 ta_sites-0.4.6/ta_sites/versant/
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-05-05 15:13:38.000000 ta_sites-0.4.6/ta_sites/versant/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-05-05 15:13:38.000000 ta_sites-0.4.6/ta_sites/versant/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10568 2023-05-05 15:13:38.000000 ta_sites-0.4.6/ta_sites/versant/requests_core.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 15:14:01.193783 ta_sites-0.4.6/ta_sites.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-05-05 15:14:01.000000 ta_sites-0.4.6/ta_sites.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      836 2023-05-05 15:14:01.000000 ta_sites-0.4.6/ta_sites.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-05 15:14:01.000000 ta_sites-0.4.6/ta_sites.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-05 15:14:01.000000 ta_sites-0.4.6/ta_sites.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-05 15:14:01.000000 ta_sites-0.4.6/ta_sites.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-05-05 15:14:01.000000 ta_sites-0.4.6/ta_sites.egg-info/top_level.txt
```

### Comparing `ta_sites-0.4.5/LICENSE` & `ta_sites-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.5/PKG-INFO` & `ta_sites-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ta_sites
-Version: 0.4.5
+Version: 0.4.6
 Summary: TA Sites
 Home-page: https://www.thoughtfulautomation.com/
 Author: Serhii Romanets
 Author-email: serhii.romanets@thoughtful.ai
 Keywords: ta_sites
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ta_sites-0.4.5/setup.py` & `ta_sites-0.4.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup_args = dict(
     name="ta_sites",
-    version="0.4.5",
+    version="0.4.6",
     packages=[
         "ta_sites",
         "ta_sites.central_reach",
         "ta_sites.basic",
         "ta_sites.quickbooks",
         "ta_sites.salesforce",
         "ta_sites.versant",
```

### Comparing `ta_sites-0.4.5/ta_sites/__init__.py` & `ta_sites-0.4.6/ta_sites/__init__.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.5/ta_sites/always_care/requests_core.py` & `ta_sites-0.4.6/ta_sites/always_care/requests_core.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.5/ta_sites/basic/core.py` & `ta_sites-0.4.6/ta_sites/basic/core.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.5/ta_sites/central_reach/__init__.py` & `ta_sites-0.4.6/ta_sites/central_reach/__init__.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.5/ta_sites/central_reach/core.py` & `ta_sites-0.4.6/ta_sites/central_reach/core.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.5/ta_sites/central_reach/exceptions.py` & `ta_sites-0.4.6/ta_sites/central_reach/exceptions.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.5/ta_sites/central_reach/requests_core.py` & `ta_sites-0.4.6/ta_sites/central_reach/requests_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,26 +80,37 @@
            or 'ScheduledMaintenanceError' with exc_message,
         If status code is 401 (unauthorized) then it will try login again
         :param response: response from request
         :param mandatory_json: bool, if True - it will check is response contain json data
         :param exc_message: text message which will be raise if response wrong
         :param re_authorize: bool, if True then it will try login again if status code is 401
         """
+        # Check if site is under scheduled maintenance
         if self.__is_scheduled_maintenance(response):
             print(exc_message, "Error")
             print("'Central Reach' site is currently unavailable due to scheduled maintenance", "Error")
             raise ScheduledMaintenanceError
 
-        elif re_authorize and response.status_code == 401:
-            self._login_to_central_reach(self.__login, self.__password)
+        # Check if response is unauthorized
+        if response.status_code == 401:
+            unauthorized_request = True
+        elif self._is_json_response(response) and response.json().get("message", "") == "Not logged in.":
+            unauthorized_request = True
+        else:
+            unauthorized_request = False
+
+        if unauthorized_request:
+            if re_authorize:
+                self._login_to_central_reach(self.__login, self.__password)
             raise BadRequestError(
                 f"{exc_message}Status Code: {response.status_code} (Unauthorized request), "
                 f"Json content: {response.json()}, Headers: {response.headers}"
             )
 
+        # Check if response is not 200 or not json
         if response.status_code != 200 or (mandatory_json and not self._is_json_response(response)):
             exc_message = exc_message + "\n" if exc_message else ""
             if self._is_json_response(response):
                 raise BadRequestError(
                     f"{exc_message}Status Code: {response.status_code}, "
                     f"Json content: {response.json()}, Headers: {response.headers}"
                 )
```

### Comparing `ta_sites-0.4.5/ta_sites/quickbooks/core.py` & `ta_sites-0.4.6/ta_sites/quickbooks/core.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.5/ta_sites/quickbooks/grouped_row.py` & `ta_sites-0.4.6/ta_sites/quickbooks/grouped_row.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.5/ta_sites/salesforce/core.py` & `ta_sites-0.4.6/ta_sites/salesforce/core.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.5/ta_sites/versant/requests_core.py` & `ta_sites-0.4.6/ta_sites/versant/requests_core.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.5/ta_sites.egg-info/PKG-INFO` & `ta_sites-0.4.6/ta_sites.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ta-sites
-Version: 0.4.5
+Version: 0.4.6
 Summary: TA Sites
 Home-page: https://www.thoughtfulautomation.com/
 Author: Serhii Romanets
 Author-email: serhii.romanets@thoughtful.ai
 Keywords: ta_sites
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ta_sites-0.4.5/ta_sites.egg-info/SOURCES.txt` & `ta_sites-0.4.6/ta_sites.egg-info/SOURCES.txt`

 * *Files identical despite different names*

