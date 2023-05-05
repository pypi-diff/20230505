# Comparing `tmp/pushcart_deploy-0.1.2.tar.gz` & `tmp/pushcart_deploy-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pushcart_deploy-0.1.2.tar", max compression
+gzip compressed data, was "pushcart_deploy-1.3.2.tar", max compression
```

## Comparing `pushcart_deploy-0.1.2.tar` & `pushcart_deploy-1.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-05-05 13:49:07.907226 pushcart_deploy-0.1.2/LICENSE
--rw-r--r--   0        0        0       80 2023-05-05 13:49:07.907226 pushcart_deploy-0.1.2/README.md
--rw-r--r--   0        0        0     1139 2023-05-05 13:49:07.911226 pushcart_deploy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      118 2023-05-05 13:49:07.911226 pushcart_deploy-0.1.2/src/pushcart_deploy/__init__.py
--rw-r--r--   0        0        0    12855 2023-05-05 13:49:07.911226 pushcart_deploy-0.1.2/src/pushcart_deploy/configuration.py
--rw-r--r--   0        0        0       79 2023-05-05 13:49:07.911226 pushcart_deploy-0.1.2/src/pushcart_deploy/databricks_api/__init__.py
--rw-r--r--   0        0        0     8550 2023-05-05 13:49:07.911226 pushcart_deploy-0.1.2/src/pushcart_deploy/databricks_api/job_settings.py
--rw-r--r--   0        0        0     4625 2023-05-05 13:49:07.911226 pushcart_deploy-0.1.2/src/pushcart_deploy/databricks_api/jobs_wrapper.py
--rw-r--r--   0        0        0     4494 2023-05-05 13:49:07.911226 pushcart_deploy-0.1.2/src/pushcart_deploy/databricks_api/repos_wrapper.py
--rw-r--r--   0        0        0     3232 2023-05-05 13:49:07.911226 pushcart_deploy-0.1.2/src/pushcart_deploy/databricks_api/secrets_wrapper.py
--rw-r--r--   0        0        0     5265 2023-05-05 13:49:07.911226 pushcart_deploy-0.1.2/src/pushcart_deploy/setup.py
--rw-r--r--   0        0        0     1104 2023-05-05 13:49:07.911226 pushcart_deploy-0.1.2/src/pushcart_deploy/validation.py
--rw-r--r--   0        0        0     1149 1970-01-01 00:00:00.000000 pushcart_deploy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-05 15:44:48.478549 pushcart_deploy-1.3.2/LICENSE
+-rw-r--r--   0        0        0       80 2023-05-05 15:44:48.478549 pushcart_deploy-1.3.2/README.md
+-rw-r--r--   0        0        0     1137 2023-05-05 15:45:56.364001 pushcart_deploy-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-05-05 15:45:56.364001 pushcart_deploy-1.3.2/src/pushcart_deploy/__init__.py
+-rw-r--r--   0        0        0    12855 2023-05-05 15:44:48.478549 pushcart_deploy-1.3.2/src/pushcart_deploy/configuration.py
+-rw-r--r--   0        0        0       79 2023-05-05 15:44:48.478549 pushcart_deploy-1.3.2/src/pushcart_deploy/databricks_api/__init__.py
+-rw-r--r--   0        0        0     8550 2023-05-05 15:44:48.478549 pushcart_deploy-1.3.2/src/pushcart_deploy/databricks_api/job_settings.py
+-rw-r--r--   0        0        0     4625 2023-05-05 15:44:48.478549 pushcart_deploy-1.3.2/src/pushcart_deploy/databricks_api/jobs_wrapper.py
+-rw-r--r--   0        0        0     4494 2023-05-05 15:44:48.478549 pushcart_deploy-1.3.2/src/pushcart_deploy/databricks_api/repos_wrapper.py
+-rw-r--r--   0        0        0     3232 2023-05-05 15:44:48.478549 pushcart_deploy-1.3.2/src/pushcart_deploy/databricks_api/secrets_wrapper.py
+-rw-r--r--   0        0        0     5265 2023-05-05 15:44:48.482549 pushcart_deploy-1.3.2/src/pushcart_deploy/setup.py
+-rw-r--r--   0        0        0     1104 2023-05-05 15:44:48.482549 pushcart_deploy-1.3.2/src/pushcart_deploy/validation.py
+-rw-r--r--   0        0        0     1149 1970-01-01 00:00:00.000000 pushcart_deploy-1.3.2/PKG-INFO
```

### Comparing `pushcart_deploy-0.1.2/LICENSE` & `pushcart_deploy-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-0.1.2/pyproject.toml` & `pushcart_deploy-1.3.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pushcart-deploy"
-version = "0.1.2"
+version = "1.3.2"
 description = "Deployment helper for pipeline configurations using Pushcart"
 authors = ["Georgel Preput <georgelpreput@mailbox.org>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
@@ -20,15 +20,15 @@
 pydantic = "^1.10.7"
 python = "^3.10"
 pyyaml = "^6.0"
 tomli = "^2.0.1"
 urllib3 = "^1"
 
 [tool.poetry.dev-dependencies]
-black = { version = "^23.1a1", allow-prereleases = true }
+black = { version = "1.3.2", allow-prereleases = true }
 hypothesis = "^6.70.1"
 ipykernel = "^6.22.0"
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 
 [tool.poetry.scripts]
```

### Comparing `pushcart_deploy-0.1.2/src/pushcart_deploy/configuration.py` & `pushcart_deploy-1.3.2/src/pushcart_deploy/configuration.py`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-0.1.2/src/pushcart_deploy/databricks_api/job_settings.py` & `pushcart_deploy-1.3.2/src/pushcart_deploy/databricks_api/job_settings.py`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-0.1.2/src/pushcart_deploy/databricks_api/jobs_wrapper.py` & `pushcart_deploy-1.3.2/src/pushcart_deploy/databricks_api/jobs_wrapper.py`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-0.1.2/src/pushcart_deploy/databricks_api/repos_wrapper.py` & `pushcart_deploy-1.3.2/src/pushcart_deploy/databricks_api/repos_wrapper.py`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-0.1.2/src/pushcart_deploy/databricks_api/secrets_wrapper.py` & `pushcart_deploy-1.3.2/src/pushcart_deploy/databricks_api/secrets_wrapper.py`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-0.1.2/src/pushcart_deploy/setup.py` & `pushcart_deploy-1.3.2/src/pushcart_deploy/setup.py`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-0.1.2/src/pushcart_deploy/validation.py` & `pushcart_deploy-1.3.2/src/pushcart_deploy/validation.py`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-0.1.2/PKG-INFO` & `pushcart_deploy-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pushcart-deploy
-Version: 0.1.2
+Version: 1.3.2
 Summary: Deployment helper for pipeline configurations using Pushcart
 License: GPL-3.0-or-later
 Author: Georgel Preput
 Author-email: georgelpreput@mailbox.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

