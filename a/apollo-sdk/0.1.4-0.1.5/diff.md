# Comparing `tmp/apollo-sdk-0.1.4.tar.gz` & `tmp/apollo-sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo-sdk-0.1.4.tar", last modified: Thu May  4 23:15:11 2023, max compression
+gzip compressed data, was "apollo-sdk-0.1.5.tar", last modified: Thu May  4 23:50:51 2023, max compression
```

## Comparing `apollo-sdk-0.1.4.tar` & `apollo-sdk-0.1.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.390741 apollo-sdk-0.1.4/
--rw-r--r--   0 abpyguru   (501) staff       (20)     3793 2023-04-29 17:42:09.000000 apollo-sdk-0.1.4/LICENSE
--rw-r--r--   0 abpyguru   (501) staff       (20)      605 2023-05-04 23:15:11.390840 apollo-sdk-0.1.4/PKG-INFO
--rw-r--r--   0 abpyguru   (501) staff       (20)     5509 2023-04-29 17:42:09.000000 apollo-sdk-0.1.4/README.md
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.378208 apollo-sdk-0.1.4/apollo/
--rw-r--r--   0 abpyguru   (501) staff       (20)     1403 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     3608 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/client.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.378683 apollo-sdk-0.1.4/apollo/connectors/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/connectors/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.379119 apollo-sdk-0.1.4/apollo/connectors/aws/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/connectors/aws/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.379497 apollo-sdk-0.1.4/apollo/connectors/google/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/connectors/google/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.380866 apollo-sdk-0.1.4/apollo/connectors/microsoft/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/connectors/microsoft/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.382199 apollo-sdk-0.1.4/apollo/connectors/openai/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/connectors/openai/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1450 2023-05-03 17:36:48.000000 apollo-sdk-0.1.4/apollo/const.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.383118 apollo-sdk-0.1.4/apollo/database/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.385133 apollo-sdk-0.1.4/apollo/database/firebase/
--rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/firebase/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/firebase/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     3494 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/firebase/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1438 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/firebase/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.385352 apollo-sdk-0.1.4/apollo/database/mongo/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/mongo/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.385588 apollo-sdk-0.1.4/apollo/database/mysql/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/mysql/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.385790 apollo-sdk-0.1.4/apollo/database/postgres/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/postgres/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.386601 apollo-sdk-0.1.4/apollo/database/supabase/
--rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/supabase/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      739 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/supabase/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1553 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/supabase/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      810 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/supabase/local.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     4197 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/exceptions.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1375 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/manager.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1194 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/resource.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.386837 apollo-sdk-0.1.4/apollo/service/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/service/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.387026 apollo-sdk-0.1.4/apollo/service/graphql/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/service/graphql/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.388657 apollo-sdk-0.1.4/apollo/service/json/
--rw-r--r--   0 abpyguru   (501) staff       (20)      754 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/service/json/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      859 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/service/json/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1154 2023-05-03 17:37:51.000000 apollo-sdk-0.1.4/apollo/service/json/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      888 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/service/json/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.388886 apollo-sdk-0.1.4/apollo/tests/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/tests/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.390551 apollo-sdk-0.1.4/apollo_sdk.egg-info/
--rw-r--r--   0 abpyguru   (501) staff       (20)      605 2023-05-04 23:15:11.000000 apollo-sdk-0.1.4/apollo_sdk.egg-info/PKG-INFO
--rw-r--r--   0 abpyguru   (501) staff       (20)     1107 2023-05-04 23:15:11.000000 apollo-sdk-0.1.4/apollo_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)        1 2023-05-04 23:15:11.000000 apollo-sdk-0.1.4/apollo_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)      266 2023-05-04 23:15:11.000000 apollo-sdk-0.1.4/apollo_sdk.egg-info/requires.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)        7 2023-05-04 23:15:11.000000 apollo-sdk-0.1.4/apollo_sdk.egg-info/top_level.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)      103 2023-05-04 23:15:11.391117 apollo-sdk-0.1.4/setup.cfg
--rw-r--r--   0 abpyguru   (501) staff       (20)     1872 2023-05-04 23:13:04.000000 apollo-sdk-0.1.4/setup.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:50:51.871346 apollo-sdk-0.1.5/
+-rw-r--r--   0 abpyguru   (501) staff       (20)     3793 2023-04-29 17:42:09.000000 apollo-sdk-0.1.5/LICENSE
+-rw-r--r--   0 abpyguru   (501) staff       (20)      609 2023-05-04 23:50:51.871452 apollo-sdk-0.1.5/PKG-INFO
+-rw-r--r--   0 abpyguru   (501) staff       (20)     5509 2023-04-29 17:42:09.000000 apollo-sdk-0.1.5/README.md
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:50:51.863296 apollo-sdk-0.1.5/apollo/
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1419 2023-05-04 23:31:49.000000 apollo-sdk-0.1.5/apollo/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     3778 2023-05-04 23:47:44.000000 apollo-sdk-0.1.5/apollo/client.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:50:51.863555 apollo-sdk-0.1.5/apollo/connectors/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/connectors/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:50:51.863828 apollo-sdk-0.1.5/apollo/connectors/aws/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/connectors/aws/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:50:51.864084 apollo-sdk-0.1.5/apollo/connectors/google/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/connectors/google/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:50:51.864355 apollo-sdk-0.1.5/apollo/connectors/microsoft/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/connectors/microsoft/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:50:51.864534 apollo-sdk-0.1.5/apollo/connectors/openai/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/connectors/openai/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1450 2023-05-03 17:36:48.000000 apollo-sdk-0.1.5/apollo/const.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:50:51.864746 apollo-sdk-0.1.5/apollo/database/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/database/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:50:51.865514 apollo-sdk-0.1.5/apollo/database/firebase/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/database/firebase/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/database/firebase/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     3494 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/database/firebase/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1438 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/database/firebase/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:50:51.865710 apollo-sdk-0.1.5/apollo/database/mongo/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/database/mongo/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:50:51.865912 apollo-sdk-0.1.5/apollo/database/mysql/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/database/mysql/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:50:51.866115 apollo-sdk-0.1.5/apollo/database/postgres/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/database/postgres/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:50:51.866840 apollo-sdk-0.1.5/apollo/database/supabase/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/database/supabase/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      739 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/database/supabase/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1553 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/database/supabase/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      810 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/database/supabase/local.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     4197 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/exceptions.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1389 2023-05-04 23:32:14.000000 apollo-sdk-0.1.5/apollo/manager.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1234 2023-05-04 23:45:20.000000 apollo-sdk-0.1.5/apollo/resource.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:50:51.867010 apollo-sdk-0.1.5/apollo/service/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/service/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:50:51.867214 apollo-sdk-0.1.5/apollo/service/graphql/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/service/graphql/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:50:51.868012 apollo-sdk-0.1.5/apollo/service/json/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      754 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/service/json/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      859 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/service/json/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1209 2023-05-04 23:48:09.000000 apollo-sdk-0.1.5/apollo/service/json/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      888 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/service/json/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:50:51.868178 apollo-sdk-0.1.5/apollo/tests/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.5/apollo/tests/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:50:51.871042 apollo-sdk-0.1.5/apollo_sdk.egg-info/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      609 2023-05-04 23:50:51.000000 apollo-sdk-0.1.5/apollo_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1107 2023-05-04 23:50:51.000000 apollo-sdk-0.1.5/apollo_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)        1 2023-05-04 23:50:51.000000 apollo-sdk-0.1.5/apollo_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)      266 2023-05-04 23:50:51.000000 apollo-sdk-0.1.5/apollo_sdk.egg-info/requires.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)        7 2023-05-04 23:50:51.000000 apollo-sdk-0.1.5/apollo_sdk.egg-info/top_level.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)      103 2023-05-04 23:50:51.871721 apollo-sdk-0.1.5/setup.cfg
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1876 2023-05-04 23:50:29.000000 apollo-sdk-0.1.5/setup.py
```

### Comparing `apollo-sdk-0.1.4/LICENSE` & `apollo-sdk-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/PKG-INFO` & `apollo-sdk-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: apollo-sdk
-Version: 0.1.4
-Summary: Build automated decision making workflows. Aggregate your AI models and data into one api.
+Version: 0.1.5
+Summary: Build automated decision making workflows by aggregating your AI models and data into one api.
 Home-page: https://github.com/apolloapi/apolloapi
 Author: Apollo API, Inc.
 Author-email: adrbrownx@gmail.com
 License: Elastic License v2
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apollo-sdk-0.1.4/README.md` & `apollo-sdk-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/__init__.py` & `apollo-sdk-0.1.5/apollo/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,10 +27,10 @@
 
 
 def get_firebase_client(service_account_key) -> AbstractFirebaseClient:
     client = import_string(FIREBASE_CLIENT_CLASS)
     return client(service_account_key)
 
 
-def get_json_client() -> AbstractRestClient:
+def get_json_client(api_key) -> AbstractRestClient:
     client = import_string(REST_CLIENT_CLASS)
-    return client
+    return client(api_key)
```

### Comparing `apollo-sdk-0.1.4/apollo/client.py` & `apollo-sdk-0.1.5/apollo/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,22 +97,26 @@
             1. Apollo.fetch_tables()
             2. Apollo.query([desc/asc], [table], [column])
         """
         cls.psql_curs = cls._manager.connect_to_prefix(db_url)
         return "Syncing data with Apollo"
 
     @classmethod
-    def use(cls, provider, *args, **kwargs):
-        if provider == "Apollo":
+    def use(cls, provider, token=None, *args, **kwargs):
+        if provider.lower() == "apollo":
             cls.model = "Apollo"
-            return f"Connected to {provider} provider, using Safety model"
+            if token:
+                cls._auth_token = token
+                print(f"Connected to {provider} provider, using Safety model")
+            else:
+                print("Please set a auth token")
         else:
             return f"Provider {provider} not found"
 
     @classmethod
     def detectText(cls, text, operator, threshold):
         if cls.model:
-            print(cls.model)
-            conn = cls._service_manager.connect()
+            # print(cls.model)
+            conn = cls._service_manager.connect(cls._auth_token)
             return conn.make_https_request({"rule": f"{text} {operator} {threshold}"})
         else:
             return "No provider connected"
```

### Comparing `apollo-sdk-0.1.4/apollo/connectors/__init__.py` & `apollo-sdk-0.1.5/apollo/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/connectors/aws/__init__.py` & `apollo-sdk-0.1.5/apollo/connectors/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/connectors/google/__init__.py` & `apollo-sdk-0.1.5/apollo/connectors/google/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/connectors/microsoft/__init__.py` & `apollo-sdk-0.1.5/apollo/connectors/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/connectors/openai/__init__.py` & `apollo-sdk-0.1.5/apollo/connectors/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/const.py` & `apollo-sdk-0.1.5/apollo/const.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/__init__.py` & `apollo-sdk-0.1.5/apollo/database/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/firebase/__init__.py` & `apollo-sdk-0.1.5/apollo/database/firebase/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/firebase/base.py` & `apollo-sdk-0.1.5/apollo/database/firebase/base.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/firebase/cloud.py` & `apollo-sdk-0.1.5/apollo/database/firebase/cloud.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/firebase/local.py` & `apollo-sdk-0.1.5/apollo/database/firebase/local.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/mongo/__init__.py` & `apollo-sdk-0.1.5/apollo/database/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/mysql/__init__.py` & `apollo-sdk-0.1.5/apollo/database/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/postgres/__init__.py` & `apollo-sdk-0.1.5/apollo/database/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/supabase/__init__.py` & `apollo-sdk-0.1.5/apollo/database/supabase/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/supabase/base.py` & `apollo-sdk-0.1.5/apollo/database/supabase/base.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/supabase/cloud.py` & `apollo-sdk-0.1.5/apollo/database/supabase/cloud.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/supabase/local.py` & `apollo-sdk-0.1.5/apollo/database/supabase/local.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/exceptions.py` & `apollo-sdk-0.1.5/apollo/exceptions.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/manager.py` & `apollo-sdk-0.1.5/apollo/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,9 +39,9 @@
     @staticmethod
     def connect_to_prefix(service_account_key):
         return get_firebase_client(service_account_key)
 
 
 class JSONConnectionManager:
     @staticmethod
-    def connect():
-        return get_json_client()
+    def connect(api_key):
+        return get_json_client(api_key)
```

### Comparing `apollo-sdk-0.1.4/apollo/resource.py` & `apollo-sdk-0.1.5/apollo/resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,13 +37,16 @@
     pass
 
 
 class JSON:
 
     # Service utility class
     _service_manager = JSONConnectionManager()
+    
+    # Token
+    _auth_token = None
 
 
 class General(Postgres, JSON):
 
     # Current LLM to be used
     model = None
```

### Comparing `apollo-sdk-0.1.4/apollo/service/__init__.py` & `apollo-sdk-0.1.5/apollo/service/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/service/graphql/__init__.py` & `apollo-sdk-0.1.5/apollo/service/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/service/json/__init__.py` & `apollo-sdk-0.1.5/apollo/service/json/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/service/json/base.py` & `apollo-sdk-0.1.5/apollo/service/json/base.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/service/json/cloud.py` & `apollo-sdk-0.1.5/apollo/service/json/cloud.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 import requests
 
 from apollo.service.json.base import AbstractRestClient
 from apollo.const import test_token
 
 
 class RestClient(AbstractRestClient):
+    def __init__(self, api_key):
+        self.api_key = api_key
+
     @staticmethod
     def make_http_request():
         return None
 
-    @staticmethod
-    def make_https_request(body):
+    def make_https_request(self, body):
         response = requests.post(
             "https://api.apolloapi.io/api/v1/apollo/",
-            headers={"Authorization": f"Token {test_token}"},
+            headers={"Authorization": f"Token {self.api_key}"},
             json=body,
             timeout=10,
         )
         return response.json()
```

### Comparing `apollo-sdk-0.1.4/apollo/service/json/local.py` & `apollo-sdk-0.1.5/apollo/service/json/local.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/tests/__init__.py` & `apollo-sdk-0.1.5/apollo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo_sdk.egg-info/PKG-INFO` & `apollo-sdk-0.1.5/apollo_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: apollo-sdk
-Version: 0.1.4
-Summary: Build automated decision making workflows. Aggregate your AI models and data into one api.
+Version: 0.1.5
+Summary: Build automated decision making workflows by aggregating your AI models and data into one api.
 Home-page: https://github.com/apolloapi/apolloapi
 Author: Apollo API, Inc.
 Author-email: adrbrownx@gmail.com
 License: Elastic License v2
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apollo-sdk-0.1.4/apollo_sdk.egg-info/SOURCES.txt` & `apollo-sdk-0.1.5/apollo_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/setup.py` & `apollo-sdk-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from setuptools import setup, find_packages
 
 setup(
     name="apollo-sdk",
-    version="0.1.4",
-    description="Build automated decision making workflows. Aggregate your AI models and data into one api.",
+    version="0.1.5",
+    description="Build automated decision making workflows by aggregating your AI models and data into one api.",
     author="Apollo API, Inc.",
     author_email="adrbrownx@gmail.com",
     packages=find_packages(),
     # package_dir={'': ''},
     url="https://github.com/apolloapi/apolloapi",
     license="Elastic License v2",
     install_requires=[
```

