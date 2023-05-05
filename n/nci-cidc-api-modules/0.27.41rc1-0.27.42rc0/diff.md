# Comparing `tmp/nci_cidc_api_modules-0.27.41rc1.tar.gz` & `tmp/nci_cidc_api_modules-0.27.42rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cidc-api-gae/cidc-api-gae/dist/.tmp-2zde2s41/nci_cidc_api_modules-0.27.41rc1.tar", last modified: Fri Apr 28 15:25:25 2023, max compression
+gzip compressed data, was "/home/runner/work/cidc-api-gae/cidc-api-gae/dist/.tmp-7xdq6_e9/nci_cidc_api_modules-0.27.42rc0.tar", last modified: Fri May  5 14:16:32 2023, max compression
```

## Comparing `nci_cidc_api_modules-0.27.41rc1.tar` & `nci_cidc_api_modules-0.27.42rc0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:25:25.000000 nci_cidc_api_modules-0.27.41rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    35182 2023-04-28 15:25:25.000000 nci_cidc_api_modules-0.27.41rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34873 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:25:25.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:25:25.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/config/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/config/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/config/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/config/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/config/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:25:25.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/csms/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/csms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/csms/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:25:25.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31379 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/models/csms_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:25:25.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/models/files/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/models/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62285 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/models/files/details.py
--rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/models/files/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/models/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)   100053 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/models/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:25:25.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/shared/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/shared/emails.py
--rw-r--r--   0 runner    (1001) docker     (123)    32453 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/shared/gcloud_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/cidc_api/shared/rest_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:25:25.000000 nci_cidc_api_modules-0.27.41rc1/nci_cidc_api_modules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    35182 2023-04-28 15:25:25.000000 nci_cidc_api_modules-0.27.41rc1/nci_cidc_api_modules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-28 15:25:25.000000 nci_cidc_api_modules-0.27.41rc1/nci_cidc_api_modules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:25:25.000000 nci_cidc_api_modules-0.27.41rc1/nci_cidc_api_modules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:25:25.000000 nci_cidc_api_modules-0.27.41rc1/nci_cidc_api_modules.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-28 15:25:25.000000 nci_cidc_api_modules-0.27.41rc1/nci_cidc_api_modules.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 15:25:25.000000 nci_cidc_api_modules-0.27.41rc1/nci_cidc_api_modules.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/requirements.modules.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 15:25:25.000000 nci_cidc_api_modules-0.27.41rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:25:25.000000 nci_cidc_api_modules-0.27.41rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-04-28 15:25:15.000000 nci_cidc_api_modules-0.27.41rc1/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    35182 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34873 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/config/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/config/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/config/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/config/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/csms/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/csms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/csms/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31379 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/models/csms_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/models/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/models/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62285 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/models/files/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/models/files/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/models/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100053 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/models/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/shared/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/shared/emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32533 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/shared/gcloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/shared/rest_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/nci_cidc_api_modules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    35182 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/nci_cidc_api_modules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/nci_cidc_api_modules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/nci_cidc_api_modules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/nci_cidc_api_modules.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/nci_cidc_api_modules.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/nci_cidc_api_modules.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/requirements.modules.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/tests/test_api.py
```

### Comparing `nci_cidc_api_modules-0.27.41rc1/LICENSE` & `nci_cidc_api_modules-0.27.42rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41rc1/PKG-INFO` & `nci_cidc_api_modules-0.27.42rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci_cidc_api_modules
-Version: 0.27.41rc1
+Version: 0.27.42rc0
 Summary: SQLAlchemy data models and configuration tools used in the NCI CIDC API
 Home-page: https://github.com/NCI-CIDC/cidc-api-gae
 License: MIT license
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `nci_cidc_api_modules-0.27.41rc1/README.md` & `nci_cidc_api_modules-0.27.42rc0/README.md`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41rc1/cidc_api/config/db.py` & `nci_cidc_api_modules-0.27.42rc0/cidc_api/config/db.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41rc1/cidc_api/config/logging.py` & `nci_cidc_api_modules-0.27.42rc0/cidc_api/config/logging.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41rc1/cidc_api/config/secrets.py` & `nci_cidc_api_modules-0.27.42rc0/cidc_api/config/secrets.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41rc1/cidc_api/config/settings.py` & `nci_cidc_api_modules-0.27.42rc0/cidc_api/config/settings.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41rc1/cidc_api/csms/auth.py` & `nci_cidc_api_modules-0.27.42rc0/cidc_api/csms/auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41rc1/cidc_api/models/csms_api.py` & `nci_cidc_api_modules-0.27.42rc0/cidc_api/models/csms_api.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41rc1/cidc_api/models/files/details.py` & `nci_cidc_api_modules-0.27.42rc0/cidc_api/models/files/details.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41rc1/cidc_api/models/files/facets.py` & `nci_cidc_api_modules-0.27.42rc0/cidc_api/models/files/facets.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41rc1/cidc_api/models/migrations.py` & `nci_cidc_api_modules-0.27.42rc0/cidc_api/models/migrations.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41rc1/cidc_api/models/models.py` & `nci_cidc_api_modules-0.27.42rc0/cidc_api/models/models.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41rc1/cidc_api/models/schemas.py` & `nci_cidc_api_modules-0.27.42rc0/cidc_api/models/schemas.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41rc1/cidc_api/shared/auth.py` & `nci_cidc_api_modules-0.27.42rc0/cidc_api/shared/auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41rc1/cidc_api/shared/emails.py` & `nci_cidc_api_modules-0.27.42rc0/cidc_api/shared/emails.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,15 @@
 # - new upload alerts, and
 # - upon intaking metadata
 # cloud-functions also emails for
 # - an inactive user being disabled in disable_inactive_users,
 # - errors from CSMS in update_cidc_from_csms,
 # - errors from kicking off permissions in grant_download_permissions, and
 # - errors from implementing permissions in worker > permissions_worker
-CIDC_MAILING_LIST = (
-    "cidc-alert@ds.dfci.harvard.edu"
-    if ENV in ("prod", "staging")
-    # use Essex alert for dev-int/dev
-    else "essex-alert@cimac-network.org"
-)
+CIDC_MAILING_LIST = "essex-alert@cimac-network.org"
 
 
 def sendable(email_template):
     """
     Adds the `send` kwarg to an email template. If send_email=True,
     send the email on function call.
     """
@@ -51,15 +46,15 @@
     html_content = f"""
     <p>Hello {user.first_n},</p>
     <p>
         Your CIMAC-CIDC Portal account has been approved! 
         To begin browsing and downloading data, visit https://portal.cimac-network.org.
     </p>
     <p>
-        <strong>Note:</strong> If you haven't already, please email cidc@jimmy.harvard.edu to request permission to view data for the trials and assays relevant to your work.</p>
+        <strong>Note:</strong> If you haven't already, please email cidc-admin@mail.nih.gov to request permission to view data for the trials and assays relevant to your work.</p>
     <p>Thanks,<br/>The CIDC Project Team</p>
     """
 
     email = {
         "to_emails": [user.email],
         "subject": subject,
         "html_content": html_content,
```

### Comparing `nci_cidc_api_modules-0.27.41rc1/cidc_api/shared/gcloud_client.py` & `nci_cidc_api_modules-0.27.42rc0/cidc_api/shared/gcloud_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -960,14 +960,15 @@
     `kw` are expected to be sendgrid json api style additional email parameters.
     """
     # Don't actually send an email if this is a test
     if TESTING or ENV == "dev":
         logger.info(f"Would send email with subject '{subject}' to {to_emails}")
         return
 
+    logger.info(f"({ENV}) Sending email to {to_emails} with subject {subject}")
     email_json = json.dumps(
         dict(to_emails=to_emails, subject=subject, html_content=html_content, **kw)
     )
 
     report = _encode_and_publish(email_json, GOOGLE_EMAILS_TOPIC)
 
     # Await confirmation that the published message was received.
```

### Comparing `nci_cidc_api_modules-0.27.41rc1/cidc_api/shared/rest_utils.py` & `nci_cidc_api_modules-0.27.42rc0/cidc_api/shared/rest_utils.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41rc1/nci_cidc_api_modules.egg-info/PKG-INFO` & `nci_cidc_api_modules-0.27.42rc0/nci_cidc_api_modules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci-cidc-api-modules
-Version: 0.27.41rc1
+Version: 0.27.42rc0
 Summary: SQLAlchemy data models and configuration tools used in the NCI CIDC API
 Home-page: https://github.com/NCI-CIDC/cidc-api-gae
 License: MIT license
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `nci_cidc_api_modules-0.27.41rc1/nci_cidc_api_modules.egg-info/SOURCES.txt` & `nci_cidc_api_modules-0.27.42rc0/nci_cidc_api_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41rc1/setup.py` & `nci_cidc_api_modules-0.27.42rc0/setup.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41rc1/tests/test_api.py` & `nci_cidc_api_modules-0.27.42rc0/tests/test_api.py`

 * *Files identical despite different names*

