# Comparing `tmp/azure_recommendations-0.3.1.tar.gz` & `tmp/azure_recommendations-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_recommendations-0.3.1.tar", last modified: Fri May  5 06:46:30 2023, max compression
+gzip compressed data, was "azure_recommendations-0.3.2.tar", last modified: Fri May  5 06:56:48 2023, max compression
```

## Comparing `azure_recommendations-0.3.1.tar` & `azure_recommendations-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 06:46:30.522383 azure_recommendations-0.3.1/
--rw-rw-rw-   0        0        0        0 2023-03-24 12:23:56.000000 azure_recommendations-0.3.1/LICENCE
--rw-rw-rw-   0        0        0      533 2023-05-05 06:46:30.520389 azure_recommendations-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-03-24 12:23:56.000000 azure_recommendations-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 06:46:30.417380 azure_recommendations-0.3.1/azure_recommendations/
--rw-rw-rw-   0        0        0      602 2023-05-05 06:46:08.000000 azure_recommendations-0.3.1/azure_recommendations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:46:30.515383 azure_recommendations-0.3.1/azure_recommendations/recommendation/
--rw-rw-rw-   0        0        0     7218 2023-05-05 06:34:46.000000 azure_recommendations-0.3.1/azure_recommendations/recommendation/__init__.py
--rw-rw-rw-   0        0        0     4848 2023-05-05 06:34:47.000000 azure_recommendations-0.3.1/azure_recommendations/recommendation/advisor_recommendations.py
--rw-rw-rw-   0        0        0    14586 2023-05-05 06:34:47.000000 azure_recommendations-0.3.1/azure_recommendations/recommendation/network_recommendations.py
--rw-rw-rw-   0        0        0    10016 2023-03-24 12:23:56.000000 azure_recommendations-0.3.1/azure_recommendations/recommendation/utils.py
--rw-rw-rw-   0        0        0    21180 2023-05-05 06:34:46.000000 azure_recommendations-0.3.1/azure_recommendations/recommendation/vm_recommendations.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:46:30.433382 azure_recommendations-0.3.1/azure_recommendations.egg-info/
--rw-rw-rw-   0        0        0      533 2023-05-05 06:46:30.000000 azure_recommendations-0.3.1/azure_recommendations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      572 2023-05-05 06:46:30.000000 azure_recommendations-0.3.1/azure_recommendations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 06:46:30.000000 azure_recommendations-0.3.1/azure_recommendations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-05 06:46:30.000000 azure_recommendations-0.3.1/azure_recommendations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-05-05 06:46:30.000000 azure_recommendations-0.3.1/azure_recommendations.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      723 2023-05-05 06:46:08.000000 azure_recommendations-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 06:46:30.522383 azure_recommendations-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 06:56:48.778175 azure_recommendations-0.3.2/
+-rw-rw-rw-   0        0        0        0 2023-03-24 12:23:56.000000 azure_recommendations-0.3.2/LICENCE
+-rw-rw-rw-   0        0        0      533 2023-05-05 06:56:48.777181 azure_recommendations-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-03-24 12:23:56.000000 azure_recommendations-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 06:56:48.666175 azure_recommendations-0.3.2/azure_recommendations/
+-rw-rw-rw-   0        0        0      602 2023-05-05 06:56:14.000000 azure_recommendations-0.3.2/azure_recommendations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:56:48.775175 azure_recommendations-0.3.2/azure_recommendations/recommendation/
+-rw-rw-rw-   0        0        0     7218 2023-05-05 06:34:46.000000 azure_recommendations-0.3.2/azure_recommendations/recommendation/__init__.py
+-rw-rw-rw-   0        0        0     4848 2023-05-05 06:34:47.000000 azure_recommendations-0.3.2/azure_recommendations/recommendation/advisor_recommendations.py
+-rw-rw-rw-   0        0        0    14586 2023-05-05 06:34:47.000000 azure_recommendations-0.3.2/azure_recommendations/recommendation/network_recommendations.py
+-rw-rw-rw-   0        0        0    10016 2023-03-24 12:23:56.000000 azure_recommendations-0.3.2/azure_recommendations/recommendation/utils.py
+-rw-rw-rw-   0        0        0    21180 2023-05-05 06:34:46.000000 azure_recommendations-0.3.2/azure_recommendations/recommendation/vm_recommendations.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:56:48.706177 azure_recommendations-0.3.2/azure_recommendations.egg-info/
+-rw-rw-rw-   0        0        0      533 2023-05-05 06:56:48.000000 azure_recommendations-0.3.2/azure_recommendations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      572 2023-05-05 06:56:48.000000 azure_recommendations-0.3.2/azure_recommendations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 06:56:48.000000 azure_recommendations-0.3.2/azure_recommendations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      142 2023-05-05 06:56:48.000000 azure_recommendations-0.3.2/azure_recommendations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-05-05 06:56:48.000000 azure_recommendations-0.3.2/azure_recommendations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      718 2023-05-05 06:56:14.000000 azure_recommendations-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 06:56:48.779176 azure_recommendations-0.3.2/setup.cfg
```

### Comparing `azure_recommendations-0.3.1/PKG-INFO` & `azure_recommendations-0.3.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure_recommendations
-Version: 0.3.1
+Version: 0.3.2
 Summary: Provides Azure recommendations
 Author-email: "dheeraj.banodha" <dheeraj.banodha@impetus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `azure_recommendations-0.3.1/azure_recommendations/__init__.py` & `azure_recommendations-0.3.2/azure_recommendations/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from azure_recommendations.recommendation import recommendation
 
 import logging
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 __author__ = 'Dheeraj Banodha'
-__version__ = '0.3.1'
+__version__ = '0.3.2'
 
 
 class az_session(recommendation):
     def __init__(self, tenant_id: str, client_id: str, client_secret: str):
         """
         :param tenant_id: tenant Id from Azure
         :param client_id: Access ID
```

### Comparing `azure_recommendations-0.3.1/azure_recommendations/recommendation/__init__.py` & `azure_recommendations-0.3.2/azure_recommendations/recommendation/__init__.py`

 * *Files identical despite different names*

### Comparing `azure_recommendations-0.3.1/azure_recommendations/recommendation/advisor_recommendations.py` & `azure_recommendations-0.3.2/azure_recommendations/recommendation/advisor_recommendations.py`

 * *Files identical despite different names*

### Comparing `azure_recommendations-0.3.1/azure_recommendations/recommendation/network_recommendations.py` & `azure_recommendations-0.3.2/azure_recommendations/recommendation/network_recommendations.py`

 * *Files identical despite different names*

### Comparing `azure_recommendations-0.3.1/azure_recommendations/recommendation/utils.py` & `azure_recommendations-0.3.2/azure_recommendations/recommendation/utils.py`

 * *Files identical despite different names*

### Comparing `azure_recommendations-0.3.1/azure_recommendations/recommendation/vm_recommendations.py` & `azure_recommendations-0.3.2/azure_recommendations/recommendation/vm_recommendations.py`

 * *Files identical despite different names*

### Comparing `azure_recommendations-0.3.1/azure_recommendations.egg-info/PKG-INFO` & `azure_recommendations-0.3.2/azure_recommendations.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-recommendations
-Version: 0.3.1
+Version: 0.3.2
 Summary: Provides Azure recommendations
 Author-email: "dheeraj.banodha" <dheeraj.banodha@impetus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `azure_recommendations-0.3.1/azure_recommendations.egg-info/SOURCES.txt` & `azure_recommendations-0.3.2/azure_recommendations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure_recommendations-0.3.1/pyproject.toml` & `azure_recommendations-0.3.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "azure_recommendations"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="dheeraj.banodha", email="dheeraj.banodha@impetus.com" },
 ]
 description = "Provides Azure recommendations"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "azure-mgmt-network >= 1.12.0"
-#    "azure-mgmt-advisor",
-#    "azure-mgmt-resource",
-#    "azure-mgmt-compute",
-#    "azure-mgmt-common",
-#    "azure-mgmt-subscription",
-#    "azure-identity"
+    "azure-mgmt-network >= 1.12.0",
+    "azure-mgmt-advisor",
+    "azure-mgmt-resource",
+    "azure-mgmt-compute",
+    "azure-mgmt-common",
+    "azure-mgmt-subscription",
+    "azure-identity"
 ]
 
 #[project.urls]
 #"Homepage" = ""
 #"Bug Tracker" = ""
```

