# Comparing `tmp/gcp_ng_helpers-0.0.5.tar.gz` & `tmp/gcp_ng_helpers-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp_ng_helpers-0.0.5.tar", last modified: Fri May  5 08:44:25 2023, max compression
+gzip compressed data, was "gcp_ng_helpers-0.0.6.tar", last modified: Fri May  5 09:13:20 2023, max compression
```

## Comparing `gcp_ng_helpers-0.0.5.tar` & `gcp_ng_helpers-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:44:25.644193 gcp_ng_helpers-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 08:44:14.000000 gcp_ng_helpers-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-05 08:44:25.644193 gcp_ng_helpers-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-05 08:44:14.000000 gcp_ng_helpers-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:44:25.644193 gcp_ng_helpers-0.0.5/gcp_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:44:14.000000 gcp_ng_helpers-0.0.5/gcp_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:44:25.644193 gcp_ng_helpers-0.0.5/gcp_helpers/cloud_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 08:44:14.000000 gcp_ng_helpers-0.0.5/gcp_helpers/cloud_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-05 08:44:14.000000 gcp_ng_helpers-0.0.5/gcp_helpers/cloud_tasks/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:44:25.644193 gcp_ng_helpers-0.0.5/gcp_helpers/functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:44:14.000000 gcp_ng_helpers-0.0.5/gcp_helpers/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-05 08:44:14.000000 gcp_ng_helpers-0.0.5/gcp_helpers/functions/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-05 08:44:14.000000 gcp_ng_helpers-0.0.5/gcp_helpers/functions/routers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:44:25.644193 gcp_ng_helpers-0.0.5/gcp_ng_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-05 08:44:25.000000 gcp_ng_helpers-0.0.5/gcp_ng_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-05 08:44:25.000000 gcp_ng_helpers-0.0.5/gcp_ng_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:44:25.000000 gcp_ng_helpers-0.0.5/gcp_ng_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-05 08:44:25.000000 gcp_ng_helpers-0.0.5/gcp_ng_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 08:44:25.000000 gcp_ng_helpers-0.0.5/gcp_ng_helpers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-05 08:44:14.000000 gcp_ng_helpers-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-05 08:44:25.644193 gcp_ng_helpers-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:13:20.662565 gcp_ng_helpers-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 09:13:04.000000 gcp_ng_helpers-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-05 09:13:20.662565 gcp_ng_helpers-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-05 09:13:04.000000 gcp_ng_helpers-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:13:20.658565 gcp_ng_helpers-0.0.6/gcp_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:13:04.000000 gcp_ng_helpers-0.0.6/gcp_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:13:20.658565 gcp_ng_helpers-0.0.6/gcp_helpers/cloud_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 09:13:04.000000 gcp_ng_helpers-0.0.6/gcp_helpers/cloud_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-05 09:13:04.000000 gcp_ng_helpers-0.0.6/gcp_helpers/cloud_tasks/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:13:20.662565 gcp_ng_helpers-0.0.6/gcp_helpers/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:13:04.000000 gcp_ng_helpers-0.0.6/gcp_helpers/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-05 09:13:04.000000 gcp_ng_helpers-0.0.6/gcp_helpers/functions/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-05 09:13:04.000000 gcp_ng_helpers-0.0.6/gcp_helpers/functions/routers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:13:20.662565 gcp_ng_helpers-0.0.6/gcp_ng_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-05 09:13:20.000000 gcp_ng_helpers-0.0.6/gcp_ng_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-05 09:13:20.000000 gcp_ng_helpers-0.0.6/gcp_ng_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:13:20.000000 gcp_ng_helpers-0.0.6/gcp_ng_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-05 09:13:20.000000 gcp_ng_helpers-0.0.6/gcp_ng_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 09:13:20.000000 gcp_ng_helpers-0.0.6/gcp_ng_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-05 09:13:04.000000 gcp_ng_helpers-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-05 09:13:20.662565 gcp_ng_helpers-0.0.6/setup.cfg
```

### Comparing `gcp_ng_helpers-0.0.5/LICENSE` & `gcp_ng_helpers-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gcp_ng_helpers-0.0.5/PKG-INFO` & `gcp_ng_helpers-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp_ng_helpers
-Version: 0.0.5
+Version: 0.0.6
 Summary: Various helper functions for Google Cloud services
 Home-page: https://github.com/NGhostClub/gcp-helpers
 Author: Dmitriy Tischenko aka NGhost
 Author-email: nghostik@gmail.com
 Project-URL: Source, https://github.com/NGhostClub/gcp-helpers
 Project-URL: Bug Tracker, https://github.com/NGhostClub/gcp-helpers/issues
 Classifier: Intended Audience :: Developers
```

### Comparing `gcp_ng_helpers-0.0.5/README.md` & `gcp_ng_helpers-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `gcp_ng_helpers-0.0.5/gcp_helpers/cloud_tasks/manager.py` & `gcp_ng_helpers-0.0.6/gcp_helpers/cloud_tasks/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                 "headers": headers if headers and isinstance(headers, dict) else {}
             }
         }
         if body:
             if isinstance(body, dict):
                 body = json.dumps(body)
                 payload['http_request']['body'] = body.encode()
-            payload['http_request']['headers'].update = {"Content-type": "application/json"}
+            payload['http_request']['headers'].update({"Content-type": "application/json"})
         if auth:
             payload['http_request']["oidc_token"] = {
                     "service_account_email": self._invoker_sa_email,
                     "audience": url
             }
 
         return payload
```

### Comparing `gcp_ng_helpers-0.0.5/gcp_helpers/functions/decorators.py` & `gcp_ng_helpers-0.0.6/gcp_helpers/functions/decorators.py`

 * *Files identical despite different names*

### Comparing `gcp_ng_helpers-0.0.5/gcp_helpers/functions/routers.py` & `gcp_ng_helpers-0.0.6/gcp_helpers/functions/routers.py`

 * *Files identical despite different names*

### Comparing `gcp_ng_helpers-0.0.5/gcp_ng_helpers.egg-info/PKG-INFO` & `gcp_ng_helpers-0.0.6/gcp_ng_helpers.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-ng-helpers
-Version: 0.0.5
+Version: 0.0.6
 Summary: Various helper functions for Google Cloud services
 Home-page: https://github.com/NGhostClub/gcp-helpers
 Author: Dmitriy Tischenko aka NGhost
 Author-email: nghostik@gmail.com
 Project-URL: Source, https://github.com/NGhostClub/gcp-helpers
 Project-URL: Bug Tracker, https://github.com/NGhostClub/gcp-helpers/issues
 Classifier: Intended Audience :: Developers
```

### Comparing `gcp_ng_helpers-0.0.5/setup.cfg` & `gcp_ng_helpers-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 license_file = LICENSE
 name = gcp_ng_helpers
-version = 0.0.5
+version = 0.0.6
 author = Dmitriy Tischenko aka NGhost
 author_email = nghostik@gmail.com
 description = Various helper functions for Google Cloud services
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/NGhostClub/gcp-helpers
 project_urls =
```

