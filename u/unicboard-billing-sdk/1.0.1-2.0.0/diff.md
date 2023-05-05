# Comparing `tmp/unicboard_billing_sdk-1.0.1.tar.gz` & `tmp/unicboard_billing_sdk-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicboard_billing_sdk-1.0.1.tar", last modified: Mon Apr  3 05:18:29 2023, max compression
+gzip compressed data, was "unicboard_billing_sdk-2.0.0.tar", last modified: Fri May  5 08:54:45 2023, max compression
```

## Comparing `unicboard_billing_sdk-1.0.1.tar` & `unicboard_billing_sdk-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 artem9751  (1000) artem9751  (1000)        0 2023-04-03 05:18:29.447836 unicboard_billing_sdk-1.0.1/
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     1062 2022-05-19 07:26:17.000000 unicboard_billing_sdk-1.0.1/LICENSE
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     1571 2023-04-03 05:18:29.447836 unicboard_billing_sdk-1.0.1/PKG-INFO
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)      895 2023-03-30 09:19:40.000000 unicboard_billing_sdk-1.0.1/README.md
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)       38 2023-04-03 05:18:29.447836 unicboard_billing_sdk-1.0.1/setup.cfg
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     1149 2023-04-03 05:16:15.000000 unicboard_billing_sdk-1.0.1/setup.py
-drwxrwxr-x   0 artem9751  (1000) artem9751  (1000)        0 2023-04-03 05:18:29.447836 unicboard_billing_sdk-1.0.1/unicboard_billing_sdk/
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)      100 2023-03-28 06:45:17.000000 unicboard_billing_sdk-1.0.1/unicboard_billing_sdk/__init__.py
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     5350 2023-04-03 05:16:15.000000 unicboard_billing_sdk-1.0.1/unicboard_billing_sdk/billing_api_sdk.py
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     6826 2023-03-27 11:57:48.000000 unicboard_billing_sdk-1.0.1/unicboard_billing_sdk/response_models.py
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     4494 2023-03-28 06:44:49.000000 unicboard_billing_sdk-1.0.1/unicboard_billing_sdk/utils.py
-drwxrwxr-x   0 artem9751  (1000) artem9751  (1000)        0 2023-04-03 05:18:29.447836 unicboard_billing_sdk-1.0.1/unicboard_billing_sdk.egg-info/
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     1571 2023-04-03 05:18:29.000000 unicboard_billing_sdk-1.0.1/unicboard_billing_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)      397 2023-04-03 05:18:29.000000 unicboard_billing_sdk-1.0.1/unicboard_billing_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)        1 2023-04-03 05:18:29.000000 unicboard_billing_sdk-1.0.1/unicboard_billing_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)       17 2023-04-03 05:18:29.000000 unicboard_billing_sdk-1.0.1/unicboard_billing_sdk.egg-info/requires.txt
--rw-rw-r--   0 artem9751  (1000) artem9751  (1000)       22 2023-04-03 05:18:29.000000 unicboard_billing_sdk-1.0.1/unicboard_billing_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 artem9751  (1000) artem9751  (1000)        0 2023-05-05 08:54:45.766350 unicboard_billing_sdk-2.0.0/
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     1062 2022-05-19 07:26:17.000000 unicboard_billing_sdk-2.0.0/LICENSE
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     1571 2023-05-05 08:54:45.766350 unicboard_billing_sdk-2.0.0/PKG-INFO
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)      895 2023-03-30 09:19:40.000000 unicboard_billing_sdk-2.0.0/README.md
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)       38 2023-05-05 08:54:45.766350 unicboard_billing_sdk-2.0.0/setup.cfg
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     1149 2023-05-05 08:53:56.000000 unicboard_billing_sdk-2.0.0/setup.py
+drwxrwxr-x   0 artem9751  (1000) artem9751  (1000)        0 2023-05-05 08:54:45.766350 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk/
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)      100 2023-05-05 05:52:15.000000 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk/__init__.py
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     9415 2023-05-05 08:51:19.000000 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk/billing_api_sdk.py
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)    12170 2023-05-05 08:51:19.000000 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk/response_models.py
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     6939 2023-05-05 08:51:19.000000 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk/utils.py
+drwxrwxr-x   0 artem9751  (1000) artem9751  (1000)        0 2023-05-05 08:54:45.766350 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk.egg-info/
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)     1571 2023-05-05 08:54:45.000000 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)      397 2023-05-05 08:54:45.000000 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)        1 2023-05-05 08:54:45.000000 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)       17 2023-05-05 08:54:45.000000 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk.egg-info/requires.txt
+-rw-rw-r--   0 artem9751  (1000) artem9751  (1000)       22 2023-05-05 08:54:45.000000 unicboard_billing_sdk-2.0.0/unicboard_billing_sdk.egg-info/top_level.txt
```

### Comparing `unicboard_billing_sdk-1.0.1/LICENSE` & `unicboard_billing_sdk-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unicboard_billing_sdk-1.0.1/PKG-INFO` & `unicboard_billing_sdk-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicboard_billing_sdk
-Version: 1.0.1
+Version: 2.0.0
 Summary: Unicboard billing api
 Home-page: https://github.com/uniclab-01/billing-api
 Author: Unic-lab
 Author-email: a.brilon@unic-lab.by
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `unicboard_billing_sdk-1.0.1/README.md` & `unicboard_billing_sdk-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `unicboard_billing_sdk-1.0.1/setup.py` & `unicboard_billing_sdk-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='unicboard_billing_sdk',
-    version='1.0.1',
+    version='2.0.0',
     description='Unicboard billing api',
     author='Unic-lab',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email='a.brilon@unic-lab.by',
     url='https://github.com/uniclab-01/billing-api',
     package_data={'': ['*.yml'], },
```

### Comparing `unicboard_billing_sdk-1.0.1/unicboard_billing_sdk.egg-info/PKG-INFO` & `unicboard_billing_sdk-2.0.0/unicboard_billing_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicboard-billing-sdk
-Version: 1.0.1
+Version: 2.0.0
 Summary: Unicboard billing api
 Home-page: https://github.com/uniclab-01/billing-api
 Author: Unic-lab
 Author-email: a.brilon@unic-lab.by
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
```

