# Comparing `tmp/databricks-sdk-0.1.3.tar.gz` & `tmp/databricks-sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks-sdk-0.1.3.tar", last modified: Wed May  3 17:47:28 2023, max compression
+gzip compressed data, was "databricks-sdk-0.1.4.tar", last modified: Fri May  5 15:06:48 2023, max compression
```

## Comparing `databricks-sdk-0.1.3.tar` & `databricks-sdk-0.1.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:47:28.338732 databricks-sdk-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    29581 2023-05-03 17:47:28.338732 databricks-sdk-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28605 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:47:28.330732 databricks-sdk-0.1.3/databricks/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:47:28.330732 databricks-sdk-0.1.3/databricks/sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)    12817 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    34304 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/dbconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)    11197 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/dbutils.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:47:28.330732 databricks-sdk-0.1.3/databricks/sdk/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/mixins/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/mixins/dbfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:47:28.330732 databricks-sdk-0.1.3/databricks/sdk/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/runtime/stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:47:28.334732 databricks-sdk-0.1.3/databricks/sdk/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/service/_internal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30457 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/service/billing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   157480 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/service/catalog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   188918 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/service/compute.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14727 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/service/files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    68249 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/service/iam.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    99652 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/service/jobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   113286 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/service/ml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19395 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/service/oauth2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    51501 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/service/pipelines.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    87514 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/service/provisioning.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24891 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/service/serving.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33670 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/service/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44357 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/service/sharing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   140031 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/service/sql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43457 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/service/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/databricks/sdk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:47:28.338732 databricks-sdk-0.1.3/databricks_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29581 2023-05-03 17:47:28.000000 databricks-sdk-0.1.3/databricks_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-03 17:47:28.000000 databricks-sdk-0.1.3/databricks_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:47:28.000000 databricks-sdk-0.1.3/databricks_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-03 17:47:28.000000 databricks-sdk-0.1.3/databricks_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 17:47:28.000000 databricks-sdk-0.1.3/databricks_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-03 17:47:28.338732 databricks-sdk-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-03 17:47:17.000000 databricks-sdk-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:48.131141 databricks-sdk-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    29581 2023-05-05 15:06:48.131141 databricks-sdk-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28605 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:48.123141 databricks-sdk-0.1.4/databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:48.127141 databricks-sdk-0.1.4/databricks/sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12817 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34351 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/dbconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/dbutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:48.127141 databricks-sdk-0.1.4/databricks/sdk/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/mixins/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/mixins/dbfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:48.127141 databricks-sdk-0.1.4/databricks/sdk/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/runtime/stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:48.127141 databricks-sdk-0.1.4/databricks/sdk/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/_internal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30457 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/billing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   157480 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/catalog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   188918 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/compute.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14727 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    68249 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/iam.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    99652 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/jobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   113286 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/ml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19395 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/oauth2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51501 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/pipelines.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    87514 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/provisioning.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24891 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/serving.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33670 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44357 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/sharing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   140031 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/sql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43457 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/service/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/databricks/sdk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:48.131141 databricks-sdk-0.1.4/databricks_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29581 2023-05-05 15:06:48.000000 databricks-sdk-0.1.4/databricks_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-05 15:06:48.000000 databricks-sdk-0.1.4/databricks_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:06:48.000000 databricks-sdk-0.1.4/databricks_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-05 15:06:48.000000 databricks-sdk-0.1.4/databricks_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 15:06:48.000000 databricks-sdk-0.1.4/databricks_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-05 15:06:48.131141 databricks-sdk-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-05 15:06:35.000000 databricks-sdk-0.1.4/setup.py
```

### Comparing `databricks-sdk-0.1.3/LICENSE` & `databricks-sdk-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/NOTICE` & `databricks-sdk-0.1.4/NOTICE`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/PKG-INFO` & `databricks-sdk-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Databricks SDK for Python (Experimental)
 Home-page: https://github.com/databricks/databricks-sdk-py
 Author: Serge Smertin
 Author-email: serge.smertin@databricks.com
 License: UNKNOWN
 Keywords: databricks sdk
 Platform: UNKNOWN
```

### Comparing `databricks-sdk-0.1.3/README.md` & `databricks-sdk-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/__init__.py` & `databricks-sdk-0.1.4/databricks/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/azure.py` & `databricks-sdk-0.1.4/databricks/sdk/azure.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/core.py` & `databricks-sdk-0.1.4/databricks/sdk/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -685,18 +685,18 @@
                  *,
                  error_code: str = None,
                  detail: str = None,
                  status: str = None,
                  scimType: str = None,
                  error: str = None,
                  **kwargs):
-        if not message and error:
+        if error:
             # API 1.2 has different response format, let's adapt
             message = error
-        if not message and detail:
+        if detail:
             # Handle SCIM error message details
             # @see https://tools.ietf.org/html/rfc7644#section-3.7.3
             if detail == "null":
                 message = "SCIM API Internal Error"
             else:
                 message = detail
             # add more context from SCIM responses
@@ -754,32 +754,34 @@
             if not len(response.content):
                 return {}
             return response.json()
         except requests.exceptions.JSONDecodeError:
             message = self._make_sense_from_html(response.text)
             if not message:
                 message = response.reason
-            raise self._make_nicer_error(message) from None
+            raise self._make_nicer_error(message=message) from None
 
     @staticmethod
     def _make_sense_from_html(txt: str) -> str:
         matchers = [r'<pre>(.*)</pre>', r'<title>(.*)</title>']
         for attempt in matchers:
             expr = re.compile(attempt, re.MULTILINE)
             match = expr.search(txt)
             if not match:
                 continue
             return match.group(1).strip()
         return txt
 
-    def _make_nicer_error(self, message: str, status_code: int = 200, **kwargs) -> DatabricksError:
+    def _make_nicer_error(self, status_code: int = 200, **kwargs) -> DatabricksError:
+        message = kwargs.get('message', 'request failed')
         is_http_unauthorized_or_forbidden = status_code in (401, 403)
         if is_http_unauthorized_or_forbidden:
             message = self._cfg.wrap_debug_info(message)
-        return DatabricksError(message, **kwargs)
+        kwargs['message'] = message
+        return DatabricksError(**kwargs)
 
     def _record_request_log(self, response: requests.Response):
         if not logger.isEnabledFor(logging.DEBUG):
             return
         request = response.request
         url = urllib.parse.urlparse(request.url)
         query = ''
```

### Comparing `databricks-sdk-0.1.3/databricks/sdk/dbconnect.py` & `databricks-sdk-0.1.4/databricks/sdk/dbconnect.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/dbutils.py` & `databricks-sdk-0.1.4/databricks/sdk/dbutils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import base64
 import json
-import logging
 import threading
 import typing
 from collections import namedtuple
 
 from .core import ApiClient, Config
 from .mixins import compute as compute_ext
 from .mixins import dbfs as dbfs_ext
@@ -122,64 +121,14 @@
     def refreshMounts(self) -> bool:
         """ Forces all machines in this cluster to refresh their mount cache,
         ensuring they receive the most recent information """
         fs = self._proxy_factory('fs')
         return fs.refreshMounts()
 
 
-class _RedactingFilter(logging.Filter):
-    """Best-effort secret redaction logger"""
-
-    def __init__(self):
-        super().__init__()
-        self._secrets = set()
-
-    def register_secret(self, secret):
-        _RedactingFilter.register()
-        self._secrets.add(secret)
-
-    def filter(self, record):
-        record.msg = self._redact(record.msg)
-        if isinstance(record.args, dict):
-            for k in record.args.keys():
-                record.args[k] = self._redact(record.args[k])
-        else:
-            record.args = tuple(self._redact(arg) for arg in record.args)
-        return True
-
-    def _redact(self, msg):
-        msg = str(msg)
-        for secrets in self._secrets:
-            msg = msg.replace(secrets, '[REDACTED]')
-        return msg
-
-    @staticmethod
-    def _has_redactor(logger) -> bool:
-        if not hasattr(logger, 'filters'):
-            return True
-        for f in logger.filters:
-            if type(f) == _RedactingFilter:
-                return True
-        return False
-
-    @staticmethod
-    def register():
-        other_loggers = list(logging.Logger.manager.loggerDict.values())
-        all_loggers = [logging.Logger.manager.root] + other_loggers
-        # inject redacting filter into every initialized logger
-        for logger in all_loggers:
-            if _RedactingFilter._has_redactor(logger):
-                # skip adding this filter twice
-                continue
-            logger.filters.append(_FILTER)
-
-
-_FILTER = _RedactingFilter()
-
-
 class _SecretsUtil:
     """Remote equivalent of secrets util"""
 
     def __init__(self, secrets_api: workspace.SecretsAPI):
         self._api = secrets_api # nolint
 
     def getBytes(self, scope: str, key: str) -> bytes:
@@ -188,19 +137,14 @@
         raw = self._api._api.do('GET', '/api/2.0/secrets/get', query=query)
         return base64.b64decode(raw['value'])
 
     def get(self, scope: str, key: str) -> str:
         """Gets the string representation of a secret value for the specified secrets scope and key."""
         val = self.getBytes(scope, key)
         string_value = val.decode()
-
-        # to comply with the expected best-effort behavior from DBR DBUtils,
-        # add secret for redaction only after dbutils.secrets.get()
-        _FILTER.register_secret(string_value)
-
         return string_value
 
     def list(self, scope) -> typing.List[SecretMetadata]:
         """Lists the metadata for secrets within the specified scope."""
 
         # transform from SDK dataclass to dbutils-compatible namedtuple
         return [SecretMetadata(v.key) for v in self._api.list_secrets(scope)]
```

### Comparing `databricks-sdk-0.1.3/databricks/sdk/mixins/compute.py` & `databricks-sdk-0.1.4/databricks/sdk/mixins/compute.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/mixins/dbfs.py` & `databricks-sdk-0.1.4/databricks/sdk/mixins/dbfs.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/oauth.py` & `databricks-sdk-0.1.4/databricks/sdk/oauth.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/runtime/__init__.py` & `databricks-sdk-0.1.4/databricks/sdk/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/runtime/stub.py` & `databricks-sdk-0.1.4/databricks/sdk/runtime/stub.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/service/_internal.py` & `databricks-sdk-0.1.4/databricks/sdk/service/_internal.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/service/billing.py` & `databricks-sdk-0.1.4/databricks/sdk/service/billing.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/service/catalog.py` & `databricks-sdk-0.1.4/databricks/sdk/service/catalog.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/service/compute.py` & `databricks-sdk-0.1.4/databricks/sdk/service/compute.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/service/files.py` & `databricks-sdk-0.1.4/databricks/sdk/service/files.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/service/iam.py` & `databricks-sdk-0.1.4/databricks/sdk/service/iam.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/service/jobs.py` & `databricks-sdk-0.1.4/databricks/sdk/service/jobs.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/service/ml.py` & `databricks-sdk-0.1.4/databricks/sdk/service/ml.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/service/oauth2.py` & `databricks-sdk-0.1.4/databricks/sdk/service/oauth2.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/service/pipelines.py` & `databricks-sdk-0.1.4/databricks/sdk/service/pipelines.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/service/provisioning.py` & `databricks-sdk-0.1.4/databricks/sdk/service/provisioning.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/service/serving.py` & `databricks-sdk-0.1.4/databricks/sdk/service/serving.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/service/settings.py` & `databricks-sdk-0.1.4/databricks/sdk/service/settings.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/service/sharing.py` & `databricks-sdk-0.1.4/databricks/sdk/service/sharing.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/service/sql.py` & `databricks-sdk-0.1.4/databricks/sdk/service/sql.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks/sdk/service/workspace.py` & `databricks-sdk-0.1.4/databricks/sdk/service/workspace.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/databricks_sdk.egg-info/PKG-INFO` & `databricks-sdk-0.1.4/databricks_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Databricks SDK for Python (Experimental)
 Home-page: https://github.com/databricks/databricks-sdk-py
 Author: Serge Smertin
 Author-email: serge.smertin@databricks.com
 License: UNKNOWN
 Keywords: databricks sdk
 Platform: UNKNOWN
```

### Comparing `databricks-sdk-0.1.3/databricks_sdk.egg-info/SOURCES.txt` & `databricks-sdk-0.1.4/databricks_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/setup.cfg` & `databricks-sdk-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.3/setup.py` & `databricks-sdk-0.1.4/setup.py`

 * *Files identical despite different names*

