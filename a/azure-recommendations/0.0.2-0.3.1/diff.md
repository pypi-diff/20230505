# Comparing `tmp/azure_recommendations-0.0.2.tar.gz` & `tmp/azure_recommendations-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_recommendations-0.0.2.tar", last modified: Fri Mar  3 09:25:45 2023, max compression
+gzip compressed data, was "azure_recommendations-0.3.1.tar", last modified: Fri May  5 06:46:30 2023, max compression
```

## Comparing `azure_recommendations-0.0.2.tar` & `azure_recommendations-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-03 09:25:45.349399 azure_recommendations-0.0.2/
--rw-rw-rw-   0        0        0        0 2022-11-22 10:22:06.000000 azure_recommendations-0.0.2/LICENCE
--rw-rw-rw-   0        0        0      511 2023-03-03 09:25:45.339701 azure_recommendations-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      150 2023-03-02 05:04:31.000000 azure_recommendations-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-03 09:25:45.224702 azure_recommendations-0.0.2/azure_recommendations/
--rw-rw-rw-   0        0        0      602 2023-03-03 09:23:04.000000 azure_recommendations-0.0.2/azure_recommendations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-03 09:25:45.331105 azure_recommendations-0.0.2/azure_recommendations/recommendation/
--rw-rw-rw-   0        0        0     2045 2023-03-02 09:31:04.000000 azure_recommendations-0.0.2/azure_recommendations/recommendation/__init__.py
--rw-rw-rw-   0        0        0     1806 2023-03-02 05:35:45.000000 azure_recommendations-0.0.2/azure_recommendations/recommendation/advisor_recommendations.py
--rw-rw-rw-   0        0        0     7979 2023-03-02 09:31:04.000000 azure_recommendations-0.0.2/azure_recommendations/recommendation/network_recommendations.py
--rw-rw-rw-   0        0        0     4369 2023-03-02 07:14:03.000000 azure_recommendations-0.0.2/azure_recommendations/recommendation/utils.py
--rw-rw-rw-   0        0        0     9393 2023-03-02 06:51:47.000000 azure_recommendations-0.0.2/azure_recommendations/recommendation/vm_recommendations.py
-drwxrwxrwx   0        0        0        0 2023-03-03 09:25:45.264914 azure_recommendations-0.0.2/azure_recommendations.egg-info/
--rw-rw-rw-   0        0        0      511 2023-03-03 09:25:45.000000 azure_recommendations-0.0.2/azure_recommendations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-03-03 09:25:45.000000 azure_recommendations-0.0.2/azure_recommendations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-03 09:25:45.000000 azure_recommendations-0.0.2/azure_recommendations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-03-03 09:25:45.000000 azure_recommendations-0.0.2/azure_recommendations.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      498 2023-03-03 09:23:19.000000 azure_recommendations-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-03 09:25:45.352506 azure_recommendations-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 06:46:30.522383 azure_recommendations-0.3.1/
+-rw-rw-rw-   0        0        0        0 2023-03-24 12:23:56.000000 azure_recommendations-0.3.1/LICENCE
+-rw-rw-rw-   0        0        0      533 2023-05-05 06:46:30.520389 azure_recommendations-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-03-24 12:23:56.000000 azure_recommendations-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 06:46:30.417380 azure_recommendations-0.3.1/azure_recommendations/
+-rw-rw-rw-   0        0        0      602 2023-05-05 06:46:08.000000 azure_recommendations-0.3.1/azure_recommendations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:46:30.515383 azure_recommendations-0.3.1/azure_recommendations/recommendation/
+-rw-rw-rw-   0        0        0     7218 2023-05-05 06:34:46.000000 azure_recommendations-0.3.1/azure_recommendations/recommendation/__init__.py
+-rw-rw-rw-   0        0        0     4848 2023-05-05 06:34:47.000000 azure_recommendations-0.3.1/azure_recommendations/recommendation/advisor_recommendations.py
+-rw-rw-rw-   0        0        0    14586 2023-05-05 06:34:47.000000 azure_recommendations-0.3.1/azure_recommendations/recommendation/network_recommendations.py
+-rw-rw-rw-   0        0        0    10016 2023-03-24 12:23:56.000000 azure_recommendations-0.3.1/azure_recommendations/recommendation/utils.py
+-rw-rw-rw-   0        0        0    21180 2023-05-05 06:34:46.000000 azure_recommendations-0.3.1/azure_recommendations/recommendation/vm_recommendations.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:46:30.433382 azure_recommendations-0.3.1/azure_recommendations.egg-info/
+-rw-rw-rw-   0        0        0      533 2023-05-05 06:46:30.000000 azure_recommendations-0.3.1/azure_recommendations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      572 2023-05-05 06:46:30.000000 azure_recommendations-0.3.1/azure_recommendations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 06:46:30.000000 azure_recommendations-0.3.1/azure_recommendations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-05 06:46:30.000000 azure_recommendations-0.3.1/azure_recommendations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-05-05 06:46:30.000000 azure_recommendations-0.3.1/azure_recommendations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      723 2023-05-05 06:46:08.000000 azure_recommendations-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 06:46:30.522383 azure_recommendations-0.3.1/setup.cfg
```

### Comparing `azure_recommendations-0.0.2/azure_recommendations/__init__.py` & `azure_recommendations-0.3.1/azure_recommendations/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from azure_recommendations.recommendation import recommendation
 
 import logging
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 __author__ = 'Dheeraj Banodha'
-__version__ = '0.0.2'
+__version__ = '0.3.1'
 
 
 class az_session(recommendation):
     def __init__(self, tenant_id: str, client_id: str, client_secret: str):
         """
         :param tenant_id: tenant Id from Azure
         :param client_id: Access ID
```

### Comparing `azure_recommendations-0.0.2/azure_recommendations.egg-info/SOURCES.txt` & `azure_recommendations-0.3.1/azure_recommendations.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENCE
 README.md
 pyproject.toml
 azure_recommendations/__init__.py
 azure_recommendations.egg-info/PKG-INFO
 azure_recommendations.egg-info/SOURCES.txt
 azure_recommendations.egg-info/dependency_links.txt
+azure_recommendations.egg-info/requires.txt
 azure_recommendations.egg-info/top_level.txt
 azure_recommendations/recommendation/__init__.py
 azure_recommendations/recommendation/advisor_recommendations.py
 azure_recommendations/recommendation/network_recommendations.py
 azure_recommendations/recommendation/utils.py
 azure_recommendations/recommendation/vm_recommendations.py
```

