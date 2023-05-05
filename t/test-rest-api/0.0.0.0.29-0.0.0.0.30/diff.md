# Comparing `tmp/test_rest_api-0.0.0.0.29.tar.gz` & `tmp/test_rest_api-0.0.0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_rest_api-0.0.0.0.29.tar", last modified: Tue Apr 18 08:16:46 2023, max compression
+gzip compressed data, was "test_rest_api-0.0.0.0.30.tar", last modified: Fri May  5 09:44:52 2023, max compression
```

## Comparing `test_rest_api-0.0.0.0.29.tar` & `test_rest_api-0.0.0.0.30.tar`

### file list

```diff
@@ -1,44 +1,52 @@
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 08:16:46.918579 test_rest_api-0.0.0.0.29/
--rw-r--r--   0 trjose     (501) staff       (20)     1067 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.29/LICENSE
--rw-r--r--   0 trjose     (501) staff       (20)    64005 2023-04-18 08:16:46.918271 test_rest_api-0.0.0.0.29/PKG-INFO
--rw-r--r--   0 trjose     (501) staff       (20)    62282 2023-04-14 16:15:06.000000 test_rest_api-0.0.0.0.29/README.md
--rw-r--r--   0 trjose     (501) staff       (20)       38 2023-04-18 08:16:46.918686 test_rest_api-0.0.0.0.29/setup.cfg
--rw-r--r--   0 trjose     (501) staff       (20)     2893 2023-04-18 08:15:30.000000 test_rest_api-0.0.0.0.29/setup.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 08:16:46.900650 test_rest_api-0.0.0.0.29/test_rest_api/
--rw-r--r--   0 trjose     (501) staff       (20)      202 2023-04-15 11:23:49.000000 test_rest_api-0.0.0.0.29/test_rest_api/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1608 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.29/test_rest_api/__main__.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 08:16:46.905697 test_rest_api-0.0.0.0.29/test_rest_api/global_variables/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.29/test_rest_api/global_variables/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1161 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.29/test_rest_api/global_variables/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)     2716 2023-04-15 03:04:30.000000 test_rest_api-0.0.0.0.29/test_rest_api/global_variables/global_variables.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 08:16:46.907986 test_rest_api-0.0.0.0.29/test_rest_api/reporting/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-25 09:45:47.000000 test_rest_api-0.0.0.0.29/test_rest_api/reporting/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)    35371 2023-04-15 11:11:29.000000 test_rest_api-0.0.0.0.29/test_rest_api/reporting/html.py
--rw-r--r--   0 trjose     (501) staff       (20)     5418 2023-04-15 11:11:54.000000 test_rest_api-0.0.0.0.29/test_rest_api/reporting/report.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 08:16:46.911323 test_rest_api-0.0.0.0.29/test_rest_api/rest_api/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:34:23.000000 test_rest_api-0.0.0.0.29/test_rest_api/rest_api/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      173 2023-04-17 11:45:13.000000 test_rest_api-0.0.0.0.29/test_rest_api/rest_api/dot_dict.py
--rw-r--r--   0 trjose     (501) staff       (20)     1824 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.29/test_rest_api/rest_api/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      423 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.29/test_rest_api/rest_api/method.py
--rw-r--r--   0 trjose     (501) staff       (20)      332 2023-04-17 12:21:54.000000 test_rest_api-0.0.0.0.29/test_rest_api/rest_api/response.py
--rw-r--r--   0 trjose     (501) staff       (20)     6174 2023-04-17 12:21:45.000000 test_rest_api-0.0.0.0.29/test_rest_api/rest_api/rest_api.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 08:16:46.913642 test_rest_api-0.0.0.0.29/test_rest_api/testing/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:03:23.000000 test_rest_api-0.0.0.0.29/test_rest_api/testing/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     3047 2023-04-16 09:12:15.000000 test_rest_api-0.0.0.0.29/test_rest_api/testing/bug.py
--rw-r--r--   0 trjose     (501) staff       (20)    15318 2023-04-18 08:14:24.000000 test_rest_api-0.0.0.0.29/test_rest_api/testing/decorator.py
--rw-r--r--   0 trjose     (501) staff       (20)      863 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.29/test_rest_api/testing/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)    13772 2023-04-15 07:27:16.000000 test_rest_api-0.0.0.0.29/test_rest_api/testing/runner.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 08:16:46.917619 test_rest_api-0.0.0.0.29/test_rest_api/utils/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.29/test_rest_api/utils/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      943 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.29/test_rest_api/utils/aiohttp_session.py
--rw-r--r--   0 trjose     (501) staff       (20)      546 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.29/test_rest_api/utils/colors.py
--rw-r--r--   0 trjose     (501) staff       (20)      247 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.29/test_rest_api/utils/decorator_hints.py
--rw-r--r--   0 trjose     (501) staff       (20)     2027 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.29/test_rest_api/utils/error_msg.py
--rw-r--r--   0 trjose     (501) staff       (20)     1130 2023-04-16 06:45:29.000000 test_rest_api-0.0.0.0.29/test_rest_api/utils/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      606 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.29/test_rest_api/utils/logger.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-18 08:16:46.903929 test_rest_api-0.0.0.0.29/test_rest_api.egg-info/
--rw-r--r--   0 trjose     (501) staff       (20)    64005 2023-04-18 08:16:46.000000 test_rest_api-0.0.0.0.29/test_rest_api.egg-info/PKG-INFO
--rw-r--r--   0 trjose     (501) staff       (20)     1112 2023-04-18 08:16:46.000000 test_rest_api-0.0.0.0.29/test_rest_api.egg-info/SOURCES.txt
--rw-r--r--   0 trjose     (501) staff       (20)        1 2023-04-18 08:16:46.000000 test_rest_api-0.0.0.0.29/test_rest_api.egg-info/dependency_links.txt
--rw-r--r--   0 trjose     (501) staff       (20)       29 2023-04-18 08:16:46.000000 test_rest_api-0.0.0.0.29/test_rest_api.egg-info/requires.txt
--rw-r--r--   0 trjose     (501) staff       (20)       14 2023-04-18 08:16:46.000000 test_rest_api-0.0.0.0.29/test_rest_api.egg-info/top_level.txt
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-05 09:44:52.227249 test_rest_api-0.0.0.0.30/
+-rw-r--r--   0 trjose     (501) staff       (20)     1067 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.30/LICENSE
+-rw-r--r--   0 trjose     (501) staff       (20)    64379 2023-05-05 09:44:52.226955 test_rest_api-0.0.0.0.30/PKG-INFO
+-rw-r--r--   0 trjose     (501) staff       (20)    62656 2023-05-02 07:11:18.000000 test_rest_api-0.0.0.0.30/README.md
+-rw-r--r--   0 trjose     (501) staff       (20)       38 2023-05-05 09:44:52.227383 test_rest_api-0.0.0.0.30/setup.cfg
+-rw-r--r--   0 trjose     (501) staff       (20)     2946 2023-05-05 09:43:30.000000 test_rest_api-0.0.0.0.30/setup.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-05 09:44:52.198647 test_rest_api-0.0.0.0.30/test_rest_api/
+-rw-r--r--   0 trjose     (501) staff       (20)      242 2023-04-25 18:38:10.000000 test_rest_api-0.0.0.0.30/test_rest_api/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1608 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.30/test_rest_api/__main__.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-05 09:44:52.202980 test_rest_api-0.0.0.0.30/test_rest_api/assertion/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-20 18:34:45.000000 test_rest_api-0.0.0.0.30/test_rest_api/assertion/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1675 2023-04-28 10:04:23.000000 test_rest_api-0.0.0.0.30/test_rest_api/assertion/assertion.py
+-rw-r--r--   0 trjose     (501) staff       (20)      107 2023-04-25 18:29:05.000000 test_rest_api-0.0.0.0.30/test_rest_api/assertion/exception.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-05 09:44:52.205098 test_rest_api-0.0.0.0.30/test_rest_api/global_variables/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.30/test_rest_api/global_variables/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      116 2023-04-25 18:28:31.000000 test_rest_api-0.0.0.0.30/test_rest_api/global_variables/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)     4044 2023-04-25 18:18:31.000000 test_rest_api-0.0.0.0.30/test_rest_api/global_variables/global_variables.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-05 09:44:52.207795 test_rest_api-0.0.0.0.30/test_rest_api/reporting/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-25 09:45:47.000000 test_rest_api-0.0.0.0.30/test_rest_api/reporting/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)    35380 2023-04-26 10:08:07.000000 test_rest_api-0.0.0.0.30/test_rest_api/reporting/html.py
+-rw-r--r--   0 trjose     (501) staff       (20)     5427 2023-04-26 10:06:51.000000 test_rest_api-0.0.0.0.30/test_rest_api/reporting/report.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-05 09:44:52.212058 test_rest_api-0.0.0.0.30/test_rest_api/rest_api/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:34:23.000000 test_rest_api-0.0.0.0.30/test_rest_api/rest_api/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      177 2023-04-25 18:31:18.000000 test_rest_api-0.0.0.0.30/test_rest_api/rest_api/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      423 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.30/test_rest_api/rest_api/method.py
+-rw-r--r--   0 trjose     (501) staff       (20)      579 2023-04-25 14:33:03.000000 test_rest_api-0.0.0.0.30/test_rest_api/rest_api/response.py
+-rw-r--r--   0 trjose     (501) staff       (20)     6616 2023-04-26 07:15:33.000000 test_rest_api-0.0.0.0.30/test_rest_api/rest_api/rest_api.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-05 09:44:52.213826 test_rest_api-0.0.0.0.30/test_rest_api/settings/
+-rw-r--r--   0 trjose     (501) staff       (20)       29 2023-04-26 09:34:57.000000 test_rest_api-0.0.0.0.30/test_rest_api/settings/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      149 2023-04-25 14:29:54.000000 test_rest_api-0.0.0.0.30/test_rest_api/settings/logging.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-05 09:44:52.219941 test_rest_api-0.0.0.0.30/test_rest_api/testing/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:03:23.000000 test_rest_api-0.0.0.0.30/test_rest_api/testing/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     3520 2023-04-28 09:43:49.000000 test_rest_api-0.0.0.0.30/test_rest_api/testing/bug.py
+-rw-r--r--   0 trjose     (501) staff       (20)    14090 2023-04-28 11:51:16.000000 test_rest_api-0.0.0.0.30/test_rest_api/testing/decorator.py
+-rw-r--r--   0 trjose     (501) staff       (20)      112 2023-04-25 18:31:32.000000 test_rest_api-0.0.0.0.30/test_rest_api/testing/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)    12905 2023-04-26 10:09:41.000000 test_rest_api-0.0.0.0.30/test_rest_api/testing/runner.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2696 2023-05-02 05:37:13.000000 test_rest_api-0.0.0.0.30/test_rest_api/testing/traceback.py
+-rw-r--r--   0 trjose     (501) staff       (20)      785 2023-04-26 09:40:30.000000 test_rest_api-0.0.0.0.30/test_rest_api/testing/utils.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-05 09:44:52.225867 test_rest_api-0.0.0.0.30/test_rest_api/utils/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.30/test_rest_api/utils/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      943 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.30/test_rest_api/utils/aiohttp_session.py
+-rw-r--r--   0 trjose     (501) staff       (20)      247 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.30/test_rest_api/utils/decorator_hints.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1369 2023-04-26 10:50:21.000000 test_rest_api-0.0.0.0.30/test_rest_api/utils/error_msg.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2032 2023-04-28 11:35:57.000000 test_rest_api-0.0.0.0.30/test_rest_api/utils/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      606 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.30/test_rest_api/utils/logger.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1322 2023-04-19 12:03:08.000000 test_rest_api-0.0.0.0.30/test_rest_api/utils/string_color.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-05 09:44:52.200929 test_rest_api-0.0.0.0.30/test_rest_api.egg-info/
+-rw-r--r--   0 trjose     (501) staff       (20)    64379 2023-05-05 09:44:52.000000 test_rest_api-0.0.0.0.30/test_rest_api.egg-info/PKG-INFO
+-rw-r--r--   0 trjose     (501) staff       (20)     1328 2023-05-05 09:44:52.000000 test_rest_api-0.0.0.0.30/test_rest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 trjose     (501) staff       (20)        1 2023-05-05 09:44:52.000000 test_rest_api-0.0.0.0.30/test_rest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 trjose     (501) staff       (20)       29 2023-05-05 09:44:52.000000 test_rest_api-0.0.0.0.30/test_rest_api.egg-info/requires.txt
+-rw-r--r--   0 trjose     (501) staff       (20)       14 2023-05-05 09:44:52.000000 test_rest_api-0.0.0.0.30/test_rest_api.egg-info/top_level.txt
```

### Comparing `test_rest_api-0.0.0.0.29/LICENSE` & `test_rest_api-0.0.0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.29/PKG-INFO` & `test_rest_api-0.0.0.0.30/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_rest_api
-Version: 0.0.0.0.29
+Version: 0.0.0.0.30
 Summary: Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests
 Home-page: https://github.com/troymjose/test_rest_api
 Author: Troy M Jose
 Author-email: 
 Project-URL: Source, https://github.com/troymjose/test_rest_api
 Project-URL: Tracker, https://github.com/troymjose/test_rest_api/issues
 Keywords: test,unittest,restapi,testframework,asyncio,async,asynchronous,testingframework,rest,api,python,python3,testing,unittesting,automation,automationtest,automationtesting,restapitest,restapitesting,restapiunittest,restapiunittesting,restapiautomation,restapiautomationtest,restapiautomationtesting,apitest,apitesting,apiunittest,apiunittesting,apiautomation,apiautomationtest,apiautomationtesting
@@ -44,26 +44,27 @@
     - [Set report path](#2-set-report-path)
     - [Set .env path](#3-set-env-path)
     - [Set hashtags](#4-set-hashtags)
     - [Project structure](#5-project-structure)
 - [Examples](#examples)
     - [My first test](#1-my-first-test)
     - [Configure my test](#2-configure-my-test)
-    - [My first logger](#3-my-first-logger)
-    - [Set global variables value](#4-set-global-variables-value)
-    - [Set global variables value as constant](#5-set-global-variables-value-as-constant)
-    - [Get global variables value](#6-get-global-variables-value)
-    - [My first bug](#7-my-first-bug)
-    - [Configure my bug](#8-configure-my-bug)
-    - [My first rest api](#9-my-first-rest-api)
-    - [Configure my rest api](#10-configure-my-rest-api)
-    - [Reuse my rest api](#11-reuse-my-rest-api)
-    - [Send my rest api](#12-send-my-rest-api)
-    - [Rest api response](#13-rest-api-response)
-    - [Demo with all the above features](#14-demo)
+    - [Replace inbuilt assert](#3-replace-inbuilt-assert)
+    - [My first log](#4-my-first-log)
+    - [Set global variables value](#5-set-global-variables-value)
+    - [Set global variables value as constant](#6-set-global-variables-value-as-constant)
+    - [Get global variables value](#7-get-global-variables-value)
+    - [My first bug](#8-my-first-bug)
+    - [Configure my bug](#9-configure-my-bug)
+    - [My first rest api](#10-my-first-rest-api)
+    - [Configure my rest api](#11-configure-my-rest-api)
+    - [Reuse my rest api](#12-reuse-my-rest-api)
+    - [Send my rest api](#13-send-my-rest-api)
+    - [Rest api response](#14-rest-api-response)
+    - [Demo with all the above features](#15-demo)
 - [Reports](#reports)
     - [My first report](#1-my-first-report)
     - [Async tests report](#2-async-tests-report)
     - [Sync tests report](#3-sync-tests-report)
     - [Sync & Async report](#4-sync-and-async-report)
     - [Multi status report](#5-multi-status-report)
     - [Multi bug report](#6-multi-bug-report)
@@ -206,15 +207,15 @@
 
 ```python
 from test_rest_api import test
 
 
 @test()
 async def my_first_test():
-    return None
+    assert 4 == 5
 ```   
 
 - Create an __async__ python function with any __custom__ name
 - Decorate the function using __@test()__
 - __Async__ python functions decoratd with __@test()__ will be auto-detected as testcase
 - __Normal__ python functions decoratd with __@test()__ will __not__ be considered as testcase
 
@@ -238,15 +239,15 @@
 
 ```python
 from test_rest_api import test
 
 
 @test(name='Custom Name', desc='Description', enabled=True, tags=['SMOKE', 'ABC'], is_async=True, execution_order='1')
 async def my_second_test():
-    return None
+    assert 4 == 5
 ```
 
 - In our first example, we used @test() decorator with __empty parameters__
 - In this example, we are __using parameters__ to configure our test function
 - This can be considered as adding __settings__ to your test function
 
 
@@ -277,38 +278,55 @@
     - Default: True
 - __execution_order__
     - Mandatory: False
     - Data Type: str
     - Expected: Custom text for ordering. This will work only when is_async = False
     - Default: 'zzzzz'
 
-<h4 id="3-my-first-logger">3. My first logger</h4>
+<h4 id="3-replace-inbuilt-assert">3. Replace inbuilt assert</h4>
 
 - - -
 
 ```python
-from test_rest_api import test, Logger
+from test_rest_api import test, Assert
 
 
 @test()
 async def my_first_logger():
-    logger = Logger()
-    logger.log("my 1st log")
-    logger.log("my 2nd log")
-    return logger 
+    # assert 4 == 5
+    Assert.equal(4, 5)
+```
+
+- Assert is same as inbuilt python assert statement
+- Using test rest api Assert class improves logging
+- Assertions done using Assert will be automatically logged in final html report
+- It is __recommended__ to use Assert instead of inbuilt assert statement for all your tests
+
+<h4 id="4-my-first-log">4. My first log</h4>
+
+- - -
+
+```python
+from test_rest_api import test
+
+
+@test()
+async def my_first_logger():
+    print('My 1st log')
+    print('My 2nd log')
+    assert 4 == 5
 ```
 
-- Loggers are used to add __custom messages__ to the final html test report
-- Create a new Logger __instance__ inside your test function```logger = Logger()```
-- Logger instance __name__ can be any custom text. Here we have used __logger__
-- Add any number of log messages using __log method__ ```logger.log("my 1st log")```
-- Return logger instance for rich test __reporting__ ```return logger```
-- It is __recommended__ to use logger for all your tests
+- Python inbuilt ```print()``` function is used to add __custom messages__ to the final html test report
+- Add print() functions inside your __test function__
+- Add any number of log messages without any limit
+- It is __recommended__ to add logs for all your tests
+- Note: ```print()``` statements will not be printed to console
 
-<h4 id="4-set-global-variables-value">4. Set global variables value</h4>
+<h4 id="5-set-global-variables-value">5. Set global variables value</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, GlobalVariables
 
 
@@ -330,15 +348,15 @@
     - Data Type: str
     - Expected: Custom name for your global variable
 - __value__
     - Mandatory: True
     - Data Type: any
     - Expected: Any python data type can be stored as global variables value
 
-<h4 id="5-set-global-variables-value-as-constant">5. Set global variables value as constant</h4>
+<h4 id="6-set-global-variables-value-as-constant">6. Set global variables value as constant</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, GlobalVariables
 
 
@@ -365,15 +383,15 @@
     - Expected: Any python data type can be stored as global variables value
 - __is_constant__
     - Mandatory: False
     - Data Type: bool
     - Expected: True or False. Provide True, to create constants
     - Default: False
 
-<h4 id="6-get-global-variables-value">6. Get global variables value</h4>
+<h4 id="7-get-global-variables-value">7. Get global variables value</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, GlobalVariables
 
 
@@ -391,15 +409,15 @@
 ```GlobalVariables.get(name='token')```
 
 - __name__
     - Mandatory: True
     - Data Type: str
     - Expected: Valid name of any saved global variable
 
-<h4 id="7-my-first-bug">7. My first bug</h4>
+<h4 id="8-my-first-bug">8. My first bug</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, Bug
 
 
@@ -410,15 +428,15 @@
 
 - Bug is used to __raise issues__ in tests
 - Add custom __checks__ in your tests to validate __rest api response__
 - If __actual result__ is not the __expected result__, just call ```Bug()```
 - This will __terminate__ the current test function execution
 - Bug __details__ can be viewed in final html test __report__
 
-<h4 id="8-configure-my-bug">8. Configure my bug</h4>
+<h4 id="9-configure-my-bug">9. Configure my bug</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, Bug, Logger
 
 
@@ -463,15 +481,15 @@
     - Default: Empty list
 - __steps_to_reproduce__
     - Mandatory: False
     - Data Type: str
     - Expected: Logger instance can be used to auto-populate this field
     - Default: Empty string
 
-<h4 id="9-my-first-rest-api">9. My first rest api</h4>
+<h4 id="10-my-first-rest-api">10. My first rest api</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, RestApi
 
 
@@ -481,15 +499,15 @@
 ```
 
 - RestApi is used __create__ rest api instance in tests
 - Here we have created a basic rest api with just the __url information__
 - This example is only about creating rest api, no __send action__ is performed here
 - We will use this __instance variable__ for sending the request in upcoming examples
 
-<h4 id="10-configure-my-rest-api">10. Configure my rest api</h4>
+<h4 id="11-configure-my-rest-api">11. Configure my rest api</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, RestApi
 
 
@@ -519,15 +537,15 @@
     - Default: {}
 - __body__
     - Mandatory: False
     - Data Type: dict
     - Expected: Provide the json request payload
     - Default: {}
 
-<h4 id="11-reuse-my-rest-api">11. Reuse my rest api</h4>
+<h4 id="12-reuse-my-rest-api">12. Reuse my rest api</h4>
 
 - - -
 
 ```python
 from test_rest_api import RestApi, GlobalVariables
 
 
@@ -547,15 +565,15 @@
 - Use python __functions__ to create a rest api which will avoid __code duplication__
 - You can __call__ a function __100__ times instead of __writing__ it __100__ times
 - In this example we have created a simple __login api__
 - All the __dynamic values__ for rest api creation can be passed as function __parameters__
 - This helps in calling the same api with __different inputs__
 - Return the __RestApi instance__ which can be used in test functions for __sending__
 
-<h4 id="12-send-my-rest-api">12. Send my rest api</h4>
+<h4 id="13-send-my-rest-api">13. Send my rest api</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, RestApi
 
 
@@ -571,15 +589,15 @@
 - Now it's time to __send__ them using http methods
 - __Supported__ http methods are GET, POST, PUT, PATCH, DELETE, OPTIONS & HEAD
 - Here we are sending the rest_api using __GET__ http method
 - All the responses (1, 2 & 3) will have the __same result__
 - Because they perform the same functionality with __different syntax__
 - Similarly, __other http methods__ can be used, with your desired syntax
 
-<h4 id="13-rest-api-response">13. Rest api response</h4>
+<h4 id="14-rest-api-response">14. Rest api response</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, RestApi
 
 
@@ -613,15 +631,15 @@
 - __response.content_type__
     - Data Type: str
     - Value: Response content type
 - __response.obj__
     - Data Type: aiohttp.ClientResponse
     - Value: Python aiohttp ClientResponse object
 
-<h4 id="14-demo">14. Demo with all the above features</h4>
+<h4 id="15-demo">15. Demo with all the above features</h4>
 
 - - -
 
 ```
 .env file
 ---------
```

### Comparing `test_rest_api-0.0.0.0.29/README.md` & `test_rest_api-0.0.0.0.30/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,27 @@
     - [Set report path](#2-set-report-path)
     - [Set .env path](#3-set-env-path)
     - [Set hashtags](#4-set-hashtags)
     - [Project structure](#5-project-structure)
 - [Examples](#examples)
     - [My first test](#1-my-first-test)
     - [Configure my test](#2-configure-my-test)
-    - [My first logger](#3-my-first-logger)
-    - [Set global variables value](#4-set-global-variables-value)
-    - [Set global variables value as constant](#5-set-global-variables-value-as-constant)
-    - [Get global variables value](#6-get-global-variables-value)
-    - [My first bug](#7-my-first-bug)
-    - [Configure my bug](#8-configure-my-bug)
-    - [My first rest api](#9-my-first-rest-api)
-    - [Configure my rest api](#10-configure-my-rest-api)
-    - [Reuse my rest api](#11-reuse-my-rest-api)
-    - [Send my rest api](#12-send-my-rest-api)
-    - [Rest api response](#13-rest-api-response)
-    - [Demo with all the above features](#14-demo)
+    - [Replace inbuilt assert](#3-replace-inbuilt-assert)
+    - [My first log](#4-my-first-log)
+    - [Set global variables value](#5-set-global-variables-value)
+    - [Set global variables value as constant](#6-set-global-variables-value-as-constant)
+    - [Get global variables value](#7-get-global-variables-value)
+    - [My first bug](#8-my-first-bug)
+    - [Configure my bug](#9-configure-my-bug)
+    - [My first rest api](#10-my-first-rest-api)
+    - [Configure my rest api](#11-configure-my-rest-api)
+    - [Reuse my rest api](#12-reuse-my-rest-api)
+    - [Send my rest api](#13-send-my-rest-api)
+    - [Rest api response](#14-rest-api-response)
+    - [Demo with all the above features](#15-demo)
 - [Reports](#reports)
     - [My first report](#1-my-first-report)
     - [Async tests report](#2-async-tests-report)
     - [Sync tests report](#3-sync-tests-report)
     - [Sync & Async report](#4-sync-and-async-report)
     - [Multi status report](#5-multi-status-report)
     - [Multi bug report](#6-multi-bug-report)
@@ -175,15 +176,15 @@
 
 ```python
 from test_rest_api import test
 
 
 @test()
 async def my_first_test():
-    return None
+    assert 4 == 5
 ```   
 
 - Create an __async__ python function with any __custom__ name
 - Decorate the function using __@test()__
 - __Async__ python functions decoratd with __@test()__ will be auto-detected as testcase
 - __Normal__ python functions decoratd with __@test()__ will __not__ be considered as testcase
 
@@ -207,15 +208,15 @@
 
 ```python
 from test_rest_api import test
 
 
 @test(name='Custom Name', desc='Description', enabled=True, tags=['SMOKE', 'ABC'], is_async=True, execution_order='1')
 async def my_second_test():
-    return None
+    assert 4 == 5
 ```
 
 - In our first example, we used @test() decorator with __empty parameters__
 - In this example, we are __using parameters__ to configure our test function
 - This can be considered as adding __settings__ to your test function
 
 
@@ -246,38 +247,55 @@
     - Default: True
 - __execution_order__
     - Mandatory: False
     - Data Type: str
     - Expected: Custom text for ordering. This will work only when is_async = False
     - Default: 'zzzzz'
 
-<h4 id="3-my-first-logger">3. My first logger</h4>
+<h4 id="3-replace-inbuilt-assert">3. Replace inbuilt assert</h4>
 
 - - -
 
 ```python
-from test_rest_api import test, Logger
+from test_rest_api import test, Assert
 
 
 @test()
 async def my_first_logger():
-    logger = Logger()
-    logger.log("my 1st log")
-    logger.log("my 2nd log")
-    return logger 
+    # assert 4 == 5
+    Assert.equal(4, 5)
+```
+
+- Assert is same as inbuilt python assert statement
+- Using test rest api Assert class improves logging
+- Assertions done using Assert will be automatically logged in final html report
+- It is __recommended__ to use Assert instead of inbuilt assert statement for all your tests
+
+<h4 id="4-my-first-log">4. My first log</h4>
+
+- - -
+
+```python
+from test_rest_api import test
+
+
+@test()
+async def my_first_logger():
+    print('My 1st log')
+    print('My 2nd log')
+    assert 4 == 5
 ```
 
-- Loggers are used to add __custom messages__ to the final html test report
-- Create a new Logger __instance__ inside your test function```logger = Logger()```
-- Logger instance __name__ can be any custom text. Here we have used __logger__
-- Add any number of log messages using __log method__ ```logger.log("my 1st log")```
-- Return logger instance for rich test __reporting__ ```return logger```
-- It is __recommended__ to use logger for all your tests
+- Python inbuilt ```print()``` function is used to add __custom messages__ to the final html test report
+- Add print() functions inside your __test function__
+- Add any number of log messages without any limit
+- It is __recommended__ to add logs for all your tests
+- Note: ```print()``` statements will not be printed to console
 
-<h4 id="4-set-global-variables-value">4. Set global variables value</h4>
+<h4 id="5-set-global-variables-value">5. Set global variables value</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, GlobalVariables
 
 
@@ -299,15 +317,15 @@
     - Data Type: str
     - Expected: Custom name for your global variable
 - __value__
     - Mandatory: True
     - Data Type: any
     - Expected: Any python data type can be stored as global variables value
 
-<h4 id="5-set-global-variables-value-as-constant">5. Set global variables value as constant</h4>
+<h4 id="6-set-global-variables-value-as-constant">6. Set global variables value as constant</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, GlobalVariables
 
 
@@ -334,15 +352,15 @@
     - Expected: Any python data type can be stored as global variables value
 - __is_constant__
     - Mandatory: False
     - Data Type: bool
     - Expected: True or False. Provide True, to create constants
     - Default: False
 
-<h4 id="6-get-global-variables-value">6. Get global variables value</h4>
+<h4 id="7-get-global-variables-value">7. Get global variables value</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, GlobalVariables
 
 
@@ -360,15 +378,15 @@
 ```GlobalVariables.get(name='token')```
 
 - __name__
     - Mandatory: True
     - Data Type: str
     - Expected: Valid name of any saved global variable
 
-<h4 id="7-my-first-bug">7. My first bug</h4>
+<h4 id="8-my-first-bug">8. My first bug</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, Bug
 
 
@@ -379,15 +397,15 @@
 
 - Bug is used to __raise issues__ in tests
 - Add custom __checks__ in your tests to validate __rest api response__
 - If __actual result__ is not the __expected result__, just call ```Bug()```
 - This will __terminate__ the current test function execution
 - Bug __details__ can be viewed in final html test __report__
 
-<h4 id="8-configure-my-bug">8. Configure my bug</h4>
+<h4 id="9-configure-my-bug">9. Configure my bug</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, Bug, Logger
 
 
@@ -432,15 +450,15 @@
     - Default: Empty list
 - __steps_to_reproduce__
     - Mandatory: False
     - Data Type: str
     - Expected: Logger instance can be used to auto-populate this field
     - Default: Empty string
 
-<h4 id="9-my-first-rest-api">9. My first rest api</h4>
+<h4 id="10-my-first-rest-api">10. My first rest api</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, RestApi
 
 
@@ -450,15 +468,15 @@
 ```
 
 - RestApi is used __create__ rest api instance in tests
 - Here we have created a basic rest api with just the __url information__
 - This example is only about creating rest api, no __send action__ is performed here
 - We will use this __instance variable__ for sending the request in upcoming examples
 
-<h4 id="10-configure-my-rest-api">10. Configure my rest api</h4>
+<h4 id="11-configure-my-rest-api">11. Configure my rest api</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, RestApi
 
 
@@ -488,15 +506,15 @@
     - Default: {}
 - __body__
     - Mandatory: False
     - Data Type: dict
     - Expected: Provide the json request payload
     - Default: {}
 
-<h4 id="11-reuse-my-rest-api">11. Reuse my rest api</h4>
+<h4 id="12-reuse-my-rest-api">12. Reuse my rest api</h4>
 
 - - -
 
 ```python
 from test_rest_api import RestApi, GlobalVariables
 
 
@@ -516,15 +534,15 @@
 - Use python __functions__ to create a rest api which will avoid __code duplication__
 - You can __call__ a function __100__ times instead of __writing__ it __100__ times
 - In this example we have created a simple __login api__
 - All the __dynamic values__ for rest api creation can be passed as function __parameters__
 - This helps in calling the same api with __different inputs__
 - Return the __RestApi instance__ which can be used in test functions for __sending__
 
-<h4 id="12-send-my-rest-api">12. Send my rest api</h4>
+<h4 id="13-send-my-rest-api">13. Send my rest api</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, RestApi
 
 
@@ -540,15 +558,15 @@
 - Now it's time to __send__ them using http methods
 - __Supported__ http methods are GET, POST, PUT, PATCH, DELETE, OPTIONS & HEAD
 - Here we are sending the rest_api using __GET__ http method
 - All the responses (1, 2 & 3) will have the __same result__
 - Because they perform the same functionality with __different syntax__
 - Similarly, __other http methods__ can be used, with your desired syntax
 
-<h4 id="13-rest-api-response">13. Rest api response</h4>
+<h4 id="14-rest-api-response">14. Rest api response</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, RestApi
 
 
@@ -582,15 +600,15 @@
 - __response.content_type__
     - Data Type: str
     - Value: Response content type
 - __response.obj__
     - Data Type: aiohttp.ClientResponse
     - Value: Python aiohttp ClientResponse object
 
-<h4 id="14-demo">14. Demo with all the above features</h4>
+<h4 id="15-demo">15. Demo with all the above features</h4>
 
 - - -
 
 ```
 .env file
 ---------
```

### Comparing `test_rest_api-0.0.0.0.29/setup.py` & `test_rest_api-0.0.0.0.30/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Get README.md details
 with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
     long_description = '\n' + f.read()
 
 # Setup
 setup(name='test_rest_api',
-      version='0.0.0.0.29',
+      version='0.0.0.0.30',
       author='Troy M Jose',
       author_email='',
       url='https://github.com/troymjose/test_rest_api',
       bugtrack_url='https://github.com/troymjose/test_rest_api/issues',
       project_urls={
           'Source': 'https://github.com/troymjose/test_rest_api',
           'Tracker': 'https://github.com/troymjose/test_rest_api/issues',
@@ -30,16 +30,16 @@
       description='Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests',
       keywords=['test', 'unittest', 'restapi', 'testframework', 'asyncio', 'async', 'asynchronous',
                 'testingframework', 'rest', 'api', 'python', 'python3', 'testing', 'unittesting', 'automation',
                 'automationtest', 'automationtesting',
                 'restapitest', 'restapitesting', 'restapiunittest', 'restapiunittesting', 'restapiautomation',
                 'restapiautomationtest', 'restapiautomationtesting', 'apitest', 'apitesting', 'apiunittest',
                 'apiunittesting', 'apiautomation', 'apiautomationtest', 'apiautomationtesting'],
-      packages=['test_rest_api', 'test_rest_api.global_variables', 'test_rest_api.reporting',
-                'test_rest_api.rest_api', 'test_rest_api.testing', 'test_rest_api.utils'],
+      packages=['test_rest_api', 'test_rest_api.global_variables', 'test_rest_api.reporting', 'test_rest_api.rest_api',
+                'test_rest_api.testing', 'test_rest_api.utils', 'test_rest_api.assertion', 'test_rest_api.settings'],
       install_requires=['aiohttp', 'Jinja2', 'python-dotenv'],
       long_description_content_type='text/markdown',
       long_description=long_description,
       classifiers=['Programming Language :: Python :: 3.8',
                    'Programming Language :: Python :: 3.9',
                    'Programming Language :: Python :: 3.10',
                    'Programming Language :: Python :: 3.11',
```

### Comparing `test_rest_api-0.0.0.0.29/test_rest_api/__main__.py` & `test_rest_api-0.0.0.0.30/test_rest_api/__main__.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.29/test_rest_api/reporting/html.py` & `test_rest_api-0.0.0.0.30/test_rest_api/reporting/html.py`

 * *Files 4% similar despite different names*

```diff
@@ -305,18 +305,18 @@
                       <td>
                         <span class="badge text-bg-light rounded-pill"
                           >{{ summary.errors.bug }}</span
                         >
                       </td>
                     </tr>
                     <tr>
-                      <td>Logger</td>
+                      <td>Assert</td>
                       <td>
                         <span class="badge text-bg-light rounded-pill"
-                          >{{ summary.errors.logger }}</span
+                          >{{ summary.errors.assertion }}</span
                         >
                       </td>
                     </tr>
                     <tr>
                       <td>Unexpected</td>
                       <td>
                         <span class="badge text-bg-light rounded-pill"
@@ -851,19 +851,19 @@
     </script>
     <!-- Summary Error Doughnut Chart -->
     <script>
       const errorDoughnutChart = document.getElementById("errorDoughnutChart");
       new Chart(errorDoughnutChart, {
         type: "doughnut",
         data: {
-          labels: ["Rest Api", "Global Variables", "Bug", "Logger", "Unexpected"],
+          labels: ["Rest Api", "Global Variables", "Bug", "Assertion", "Unexpected"],
           datasets: [
             {
               label: "Type",
-              data: [{{ summary.errors.rest_api }}, {{ summary.errors.global_variables }}, {{ summary.errors.bug }}, {{ summary.errors.logger }}, {{ summary.errors.unexpected }}],
+              data: [{{ summary.errors.rest_api }}, {{ summary.errors.global_variables }}, {{ summary.errors.bug }}, {{ summary.errors.assertion }}, {{ summary.errors.unexpected }}],
               backgroundColor: [
                 "rgba(255, 205, 86, 0.1)",
                 "rgba(255, 205, 86, 0.3)",
                 "rgba(255, 205, 86, 0.5)",
                 "rgba(255, 205, 86, 0.7)",
                 "rgba(255, 205, 86, 1)"
               ],
```

#### html2text {}

```diff
@@ -35,15 +35,15 @@
 Critical {{ summary.bugs.critical }}
 Blocker  {{ summary.bugs.blocker }}
   Errors
 Total            {{ summary.errors.total }}
 Rest Api         {{ summary.errors.rest_api }}
 Global Variables {{ summary.errors.global_variables }}
 Bug              {{ summary.errors.bug }}
-Logger           {{ summary.errors.logger }}
+Assert           {{ summary.errors.assertion }}
 Unexpected       {{ summary.errors.unexpected }}
 {% if summary.tests.sync_tests > 0 %}
 
 
 
   Synchronous Tests
 [Unknown INPUT type]
```

### Comparing `test_rest_api-0.0.0.0.29/test_rest_api/reporting/report.py` & `test_rest_api-0.0.0.0.30/test_rest_api/reporting/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 @dataclass
 class ErrorType:
     REST_API: str = 'rest_api'
     GLOBAL_VARIABLES: str = 'global_variables'
     BUG: str = 'bug'
-    LOGGER: str = 'logger'
+    ASSERTION: str = 'assertion'
     UNEXPECTED: str = 'unexpected'
 
 
 @dataclass
 class ReportTestResult:
     name: str
     desc: str
@@ -76,15 +76,15 @@
 
 @dataclass
 class ReportTestSummaryErrors:
     total: int = 0
     rest_api: int = 0
     global_variables: int = 0
     bug: int = 0
-    logger: int = 0
+    assertion: int = 0
     unexpected: int = 0
 
 
 @dataclass
 class ReportTestSummary:
     test: ReportTestSummaryTest = ReportTestSummaryTest()
     tests: ReportTestSummaryTests = ReportTestSummaryTests()
```

### Comparing `test_rest_api-0.0.0.0.29/test_rest_api/rest_api/rest_api.py` & `test_rest_api-0.0.0.0.30/test_rest_api/rest_api/rest_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 from dataclasses import asdict
 from aiohttp.client_exceptions import ClientConnectorError, InvalidURL, ContentTypeError
+from .. import settings
 from .method import RestApiMethod
 from ..utils.error_msg import ErrorMsg
 from ..utils.aiohttp_session import AioHttpSession
 from .response import RestApiResponse, ClientResponse
+from ..utils.exception import catch_exc, catch_exc_async
 from .exception import RestApiSendException, RestApiCreationException
 
 
-class RestApiMeta(type):
+class RestApi:
     """
-    Meta class for raising RestApiCreationException
+    Class for creating rest api instances
     """
-
-    # Calls for each instance creation
-    def __call__(cls, *args, **kwargs):
-        try:
-            cls._instance = super().__call__(*args, **kwargs)
-        except Exception as e:
-            # Catch python class instance creation exceptions
-            raise RestApiCreationException(msg=str(e).replace('RestApi.__init__()', '').strip().capitalize())
-        # Validate _instance url, parameters, headers and body
-        cls._validate()
-        # Return the instance
-        return cls._instance
+    # Create a frozen instance of RestApiMethod, so that it can be used as a constant in code
+    METHODS = RestApiMethod()
 
     def _validate(self):
         """
         Validate url, parameters, headers and body
         """
         self._validate_url()
         self._validate_parameters_and_headers()
@@ -34,143 +26,154 @@
 
     def _validate_url(self):
         """
         Checks
         ------
         1. Valid string
         """
-        if not isinstance(self._instance.url, str):
-            raise RestApiCreationException(msg='Invalid data type for url. Please provide a valid string')
+        if not isinstance(self.url, str):
+            raise Exception('Invalid data type for url. Please provide a valid string')
 
     def _validate_parameters_and_headers(self):
         """
         Checks
         ------
         1. Valid dictionary
         2. Valid dictionary schema
         """
         error = 'Please provide a valid dictionary, with both dictionary key and dictionary value as string type'
         for item in ('parameters', 'headers'):
-            if not isinstance(getattr(self._instance, item), dict):
-                raise RestApiCreationException(msg=f'Invalid data type for {item}. {error}')
+            if not isinstance(getattr(self, item), dict):
+                raise Exception(f'Invalid data type for {item}. {error}')
             if not all([isinstance(key, str) and isinstance(key, str) for key, value in
-                        getattr(self._instance, item).items()]):
-                raise RestApiCreationException(msg=f'Invalid dictionary for {item}. {error}')
+                        getattr(self, item).items()]):
+                raise Exception(f'Invalid dictionary for {item}. {error}')
 
     def _validate_body(self):
         """
         Checks
         ------
         1. Valid dictionary
         """
-        if not isinstance(self._instance.body, dict):
-            raise RestApiCreationException(msg='Invalid data type for body. Please provide a valid dictionary')
-
-
-class RestApi(metaclass=RestApiMeta):
-    """
-    Class for creating rest api instances
-    """
-    # Create a frozen instance of RestApiMethod, so that it can be used as a constant in code
-    METHODS = RestApiMethod()
+        if not isinstance(self.body, dict):
+            raise Exception('Invalid data type for body. Please provide a valid dictionary')
 
+    @catch_exc(test_rest_api_exception=RestApiCreationException)
     def __init__(self, url: str, parameters: dict = {}, headers: dict = {}, body: dict = {}):
         # Rest api variables
         self.url = url
         self.parameters = parameters
         self.headers = headers
         self.body = body
-        # Aiohttp variables
+        # Validate url, parameters, headers and body
+        self._validate()
+        # Aiohttp session
         self._session = AioHttpSession()
+        # Logging
+        print(f'\nRest Api Created\n----------------{self}')
 
     def __str__(self):
         return f"""
-Url:        {self.url}
-Headers:    {self.headers}
-Parameters: {self.parameters}
-Body:       {self.body}
+ {settings.logging.sub_point} Url        {settings.logging.key_val_sep} {self.url}
+ {settings.logging.sub_point} Headers    {settings.logging.key_val_sep} {self.headers}
+ {settings.logging.sub_point} Parameters {settings.logging.key_val_sep} {self.parameters}
+ {settings.logging.sub_point} Body       {settings.logging.key_val_sep} {self.body}
 """
 
-    async def send(self, method: str):
+    async def _create_response(self, response: ClientResponse) -> RestApiResponse:
+        """
+        Create response instance object from aiohttp async response
+        """
+        # Retrieve the response body in JSON
+        body = await response.json()
+        # Get the other response parameters
+        status_code, headers, content_type = response.status, dict(response.headers), response.content_type
+        # Create and return the RestApiResponse instance object
+        rest_api_response = RestApiResponse(status_code=status_code,
+                                            content_type=content_type,
+                                            body=body,
+                                            headers=headers,
+                                            obj=response)
+        # Logging
+        print(f'Rest Api Response\n-----------------{rest_api_response} ')
+        return rest_api_response
+
+    async def _send(self, method: str):
         """
         Send the rest api by providing the request method
         """
         try:
+            # Logging
+            print(
+                f'Rest Api Send\n-------------\n {settings.logging.sub_point} Method     {settings.logging.key_val_sep} {method.upper()}\n')
             # Check if method is of type string
             if not isinstance(method, str):
                 raise Exception('Invalid data type for method. Please provide a valid string')
             # Convert to lowercase
             method = method.lower()
             # Check if the method is valid
             if method not in asdict(self.METHODS).values():
                 raise Exception(ErrorMsg.INVALID_METHOD)
             # Send the request
             async with getattr(self._session, method)(url=self.url,
                                                       params=self.parameters,
                                                       headers=self.headers,
                                                       json=self.body) as response:
                 return await self._create_response(response=response)
-        except ClientConnectorError as exc:
-            raise RestApiSendException(msg=str(exc))
-        except InvalidURL as exc:
-            raise RestApiSendException(msg='Invalid ULR')
-        except ContentTypeError as exc:
-            raise RestApiSendException(msg=str(exc))
+        except ClientConnectorError:
+            raise Exception(ErrorMsg.CLIENT_CONNECTOR_ERROR)
+        except InvalidURL:
+            raise Exception(ErrorMsg.INVALID_URL)
+        except ContentTypeError:
+            raise Exception(ErrorMsg.INVALID_JSON_RESPONSE)
         except Exception as exc:
-            raise RestApiSendException(msg=str(exc))
+            raise exc
 
-    async def _create_response(self, response: ClientResponse) -> RestApiResponse:
+    @catch_exc_async(test_rest_api_exception=RestApiSendException)
+    async def send(self, method: str):
         """
-        Create response instance object from aiohttp async response
+        Send the rest api by providing the request method
         """
-        # Retrieve the response body in JSON
-        body = await response.json()
-        # Get the other response parameters
-        status_code, headers, content_type = response.status, dict(response.headers), response.content_type
-        # Create and return the RestApiResponse instance object
-        return RestApiResponse(status_code=status_code,
-                               content_type=content_type,
-                               body=body,
-                               headers=headers,
-                               obj=response)
+        return await self._send(method=method)
 
+    @catch_exc_async(test_rest_api_exception=RestApiSendException)
     async def get(self):
         """
         Send HTTP GET Request
         """
-        return await self.send(method=self.METHODS.GET)
+        return await self._send(method=self.METHODS.GET)
 
     async def post(self):
         """
         Send HTTP POST Request
         """
-        return await self.send(method=self.METHODS.POST)
+        return await self._send(method=self.METHODS.POST)
 
     async def put(self):
         """
         Send HTTP PUT Request
         """
-        return await self.send(method=self.METHODS.PUT)
+        return await self._send(method=self.METHODS.PUT)
 
     async def patch(self):
         """
         Send HTTP PATCH Request
         """
-        return await self.send(method=self.METHODS.PATCH)
+        return await self._send(method=self.METHODS.PATCH)
 
     async def delete(self):
         """
         Send HTTP DELETE Request
         """
-        return await self.send(method=self.METHODS.DELETE)
+        return await self._send(method=self.METHODS.DELETE)
 
     async def head(self):
         """
         Send HTTP HEAD Request
         """
-        return await self.send(method=self.METHODS.HEAD)
+        return await self._send(method=self.METHODS.HEAD)
 
     async def options(self):
         """
         Send HTTP OPTIONS Request
         """
-        return await self.send(method=self.METHODS.OPTIONS)
+        return await self._send(method=self.METHODS.OPTIONS)
```

### Comparing `test_rest_api-0.0.0.0.29/test_rest_api/testing/bug.py` & `test_rest_api-0.0.0.0.30/test_rest_api/testing/bug.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import dataclass, asdict
-from .exception import BugCreationException
+from .. import settings
 from ..utils.exception import catch_exc
+from .exception import BugCreationException
 
 
 @dataclass(frozen=True)
 class BugPriority:
     """
     Supported bug priority values
     """
@@ -63,26 +64,27 @@
                  message: str = "",
                  expected_result: str = "",
                  actual_result: str = "",
                  steps_to_reproduce: str = ""):
         # Default data for empty data
         self._no_data_to_display = 'No data to display'
         # Save all attributes to the instance
-        self.priority = priority.lower()
+        self.priority = priority
         self.message = message
         self.expected_result = expected_result
         self.actual_result = actual_result
         self.steps_to_reproduce = steps_to_reproduce
         # Validate message, priority, actual_result, expected_result and steps_to_reproduce
         self._validate()
+        # Convert the priority to lower case and also perform trim
+        self.priority = self.priority.lower().strip()
         # Exception message
         self.exc_message = f"""
-
 BUG
 ---
-Priority           : {priority.strip() if priority else self._no_data_to_display}
-Message            : {message.strip() if message else self._no_data_to_display}
-Expected result    : {expected_result.strip() if expected_result else self._no_data_to_display}
-Actual result      : {actual_result.strip() if actual_result else self._no_data_to_display}
-Steps to reproduce : {steps_to_reproduce.strip() if steps_to_reproduce else self._no_data_to_display}
+ {settings.logging.sub_point} Priority           {settings.logging.key_val_sep} {self.priority if self.priority else self._no_data_to_display}
+ {settings.logging.sub_point} Message            {settings.logging.key_val_sep} {self.message.strip() if self.message else self._no_data_to_display}
+ {settings.logging.sub_point} Expected result    {settings.logging.key_val_sep} {self.expected_result.strip() if self.expected_result else self._no_data_to_display}
+ {settings.logging.sub_point} Actual result      {settings.logging.key_val_sep} {self.actual_result.strip() if self.actual_result else self._no_data_to_display}
+ {settings.logging.sub_point} Steps to reproduce {settings.logging.key_val_sep} {self.steps_to_reproduce.strip() if self.steps_to_reproduce else self._no_data_to_display}
 """
         super().__init__(self.exc_message)
```

### Comparing `test_rest_api-0.0.0.0.29/test_rest_api/testing/decorator.py` & `test_rest_api-0.0.0.0.30/test_rest_api/testing/decorator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,220 +1,209 @@
-import re
 import traceback
 import functools
 from io import StringIO
 from itertools import count
 from datetime import datetime
 from time import perf_counter_ns
 from contextlib import redirect_stdout
 from inspect import iscoroutinefunction
 from .bug import Bug
-from ..utils.colors import colors
+from .utils import skip_test
+from .traceback import format_traceback
+from ..utils.string_color import str_color
 from .exception import BugCreationException
 from ..utils.logger import test_rest_api_logger
+from ..assertion.exception import AssertException
+from ..utils.exception import TestRestApiException
 from ..global_variables.exception import GlobalVariablesException
 from ..reporting.report import report, ReportTestResult, TestStatus, ErrorType
 from ..rest_api.exception import RestApiCreationException, RestApiSendException
 
 # Iter for creating id for testcase name
 iter_test_name = count(start=1)
 
 
-def test(*, name="", desc="", enabled=True, tags=[], is_async=True, execution_order='zzzzz'):
+def test(*, name="", desc="", enabled=True, tags=[], is_async=True, execution_order='z'):
     def testcase_decorator(func):
         @functools.wraps(func)
         async def inner(*args, **kwargs):
             # Get the test file path
             testsuite: str = func.__module__ if func.__module__ else 'root file'
-            # Create the test name
-            testcase_name: str = f'{name} ({testsuite})' if name else f'{func.__name__} ({testsuite})'
-            # Add unique id to the name (Users can provide same name for multiple testcases)
-            testcase_name += f" [{next(iter_test_name)}]"
-            # Start the stopwatch / counter
-            timer_start = perf_counter_ns()
-            # Get the start date time of the test
-            start = datetime.now().strftime('%Y-%m-%d %H-%M-%S')
-            # Initialise test status, test details and test logs
-            status, details, logs = TestStatus.SKIP, 'Testcase is skipped', 'No data to display'
-            # Initialise bug priority and error type which will be used for reporting
-            bug_priority, error_type = '', ''
-            # Initialise skip as false
-            skip = False
-            # Get the runner test tags
-            from test_rest_api import runner
-            # If we have any runner test tags
-            if runner.test_tags:
-                # Check if the tag is #ALL (This will run for all tag cases, eg: login api)
-                if 'ALL' not in tags:
-                    # Check if any of the runner test tag is present in the current test else skip the test
-                    if not any(test_tag in tags for test_tag in runner.test_tags):
-                        skip = True
-            if not skip:
-                # Initialise test status and test details
+            # Create the test name & also add unique id at the end (Users can provide same name for multiple testcases)
+            testcase_name: str = f'{name} ({testsuite})' if name else f'{func.__name__} ({testsuite})' + f' [{next(iter_test_name)}]'
+            # Initialise variables required for reporting
+            start = end = bug_priority = error_type = logs_end = ''
+            duration, logs = '0 seconds', 'No data to display'
+            # Set Skip details
+            status, details = TestStatus.SKIP, 'Testcase is skipped'
+            # Skip the test if execution #tags not present in test #tags
+            if not skip_test(tags=tags):
+                # Set Disable details
                 status, details = TestStatus.DISABLE, 'Testcase is disabled'
                 # Only execute enabled testcases
                 if enabled:
+                    # Update the logs
+                    logs = 'Started the test\n'
                     # In-memory file-like object
                     string_io = StringIO()
                     try:
+                        # Start the stopwatch / counter
+                        timer_start = perf_counter_ns()
+                        # Get the start date time of the test
+                        start = datetime.now().strftime('%Y-%m-%d %H-%M-%S')
                         # Redirect standard output to string_io
                         # In python, print() function prints values to standard out
                         with redirect_stdout(string_io):
                             # Call the async test function
                             await func(*args, **kwargs)
-                        # Log the result
-                        test_rest_api_logger.info(
-                            f"{colors.LIGHT_GREEN}{'PASS' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
+                        # Log the result to the console
+                        test_rest_api_logger.info(str_color.passed(testcase_name))
+                        # Update the logs, which has to be added after stdout (eg: error, bug etc)
+                        logs_end = 'Completed the test'
                         # Update the test status and details
                         status, details = TestStatus.PASS, 'Success'
                     except RestApiCreationException as exc:
-                        # Log the result
-                        test_rest_api_logger.info(
-                            f"{colors.YELLOW}{'ERROR' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
+                        # Log the result to the console
+                        test_rest_api_logger.info(str_color.error(testcase_name))
+                        # Update the logs, which has to be added after stdout (eg: error, bug etc)
+                        logs_end = str(exc)
                         # Update the error type for reporting
                         error_type = ErrorType.REST_API
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
-                        # Format the traceback (Remove unwanted info)
-                        start_res = re.search(r'test_rest_api(.*?)testing(.*?)decorator.py", line (.*?), in inner',
-                                              traceback_data)
-                        end_res = re.search(r'raise RestApiCreationException', traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 103:end_res.end()]
-                        traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
-                        if re.search(r'test_rest_api(.*?)rest_api(.*?)rest_api.py", line (.*?), in __call__',
-                                     traceback_data):
-                            traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
-                            traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
+                        # Format the traceback data to remove unwanted info
+                        traceback_data = format_traceback.test_rest_api_exc(traceback=traceback_data)
                         # Update the test status and details
-                        status, details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
+                        status, details = TestStatus.ERROR, traceback_data
                     except RestApiSendException as exc:
-                        # Log the result
-                        test_rest_api_logger.info(
-                            f"{colors.YELLOW}{'ERROR' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
+                        # Log the result to the console
+                        test_rest_api_logger.info(str_color.error(testcase_name))
+                        # Update the logs, which has to be added after stdout (eg: error, bug etc)
+                        logs_end = str(exc)
                         # Update the error type for reporting
                         error_type = ErrorType.REST_API
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
-                        # Format the traceback (Remove unwanted info)
-                        start_res = re.search(r'test_rest_api(.*?)testing(.*?)decorator.py", line (.*?), in inner',
-                                              traceback_data)
-                        end_res = re.search(r'raise RestApiSendException', traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 103:end_res.end()]
-                        traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
-                        traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
+                        # Format the traceback data to remove unwanted info
+                        traceback_data = format_traceback.test_rest_api_exc(traceback=traceback_data)
                         # Update the test status and details
-                        status, details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
+                        status, details = TestStatus.ERROR, traceback_data
                     except BugCreationException as exc:
-                        # Log the result
-                        test_rest_api_logger.info(
-                            f"{colors.YELLOW}{'ERROR' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
+                        # Log the result to the console
+                        test_rest_api_logger.info(str_color.error(testcase_name))
+                        # Update the logs, which has to be added after stdout (eg: error, bug etc)
+                        logs_end = str(exc)
                         # Update the error type for reporting
                         error_type = ErrorType.BUG
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
-                        # Format the traceback (Remove unwanted info)
-                        start_res = re.search(r'test_rest_api(.*?)testing(.*?)decorator.py", line (.*?), in inner',
-                                              traceback_data)
-                        end_res = re.search(r'raise test_rest_api_exception', traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 103:end_res.end()]
-                        traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
+                        # Format the traceback data to remove unwanted info
+                        traceback_data = format_traceback.test_rest_api_exc(traceback=traceback_data)
                         # Update the test status and details
-                        status, details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
+                        status, details = TestStatus.ERROR, traceback_data
                     except GlobalVariablesException as exc:
-                        # Log the result
-                        test_rest_api_logger.info(
-                            f"{colors.YELLOW}{'ERROR' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
+                        # Log the result to the console
+                        test_rest_api_logger.info(str_color.error(testcase_name))
+                        # Update the logs, which has to be added after stdout (eg: error, bug etc)
+                        logs_end = str(exc)
                         # Update the error type for reporting
                         error_type = ErrorType.GLOBAL_VARIABLES
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
-                        # Format the traceback (Remove unwanted info)
-                        start_res = re.search(r'test_rest_api(.*?)testing(.*?)decorator.py", line (.*?), in inner',
-                                              traceback_data)
-                        end_res = re.search(r'raise test_rest_api_exception', traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 103:end_res.end()]
-                        traceback_data = traceback_data[:traceback_data.rfind('File "') - 3]
+                        # Format the traceback data to remove unwanted info
+                        traceback_data = format_traceback.test_rest_api_exc(traceback=traceback_data)
                         # Update the test status and details
-                        status, details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
+                        status, details = TestStatus.ERROR, traceback_data
                     except Bug as exc:
-                        # Log the result
-                        test_rest_api_logger.info(
-                            f"{colors.LIGHT_RED}{'FAIL' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
+                        # Log the result to the console
+                        test_rest_api_logger.info(str_color.failed(testcase_name))
+                        # Update the logs, which has to be added after stdout (eg: error, bug etc)
+                        logs_end = str(exc)
                         # Update the bug priority for reporting
                         bug_priority = exc.priority
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
-                        # Format the traceback (Remove unwanted info)
-                        start_res = re.search(r'test_rest_api(.*?)testing(.*?)decorator.py", line (.*?), in inner',
-                                              traceback_data)
-                        end_res = re.search(r'raise Bug', traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 103:end_res.end()]
+                        # Format the traceback data to remove unwanted info
+                        traceback_data = format_traceback.bug_exc(traceback=traceback_data)
                         # Update the test status and details
-                        status, details = TestStatus.FAIL, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
+                        status, details = TestStatus.FAIL, traceback_data
+                    except AssertException as exc:
+                        # Log the result to the console
+                        test_rest_api_logger.info(str_color.error(testcase_name))  # Get the code traceback details
+                        # Update the logs, which has to be added after stdout (eg: error, bug etc)
+                        logs_end = str(exc)
+                        # Update the error type for reporting
+                        error_type = ErrorType.ASSERTION
+                        # Get the code traceback details
+                        traceback_data = traceback.format_exc()
+                        # Format the traceback data to remove unwanted info
+                        traceback_data = format_traceback.assert_exc(traceback=traceback_data)
+                        # Update the test status and details
+                        status, details = TestStatus.ERROR, traceback_data
                     except AssertionError as exc:
-                        # Log the result
-                        test_rest_api_logger.info(
-                            f"{colors.LIGHT_RED}{'FAIL' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
+                        # Log the result to the console
+                        test_rest_api_logger.info(str_color.failed(testcase_name))
+                        # Update the logs, which has to be added after stdout (eg: error, bug etc)
+                        logs_end = str(exc)
                         # Update the bug priority for reporting
                         bug_priority = exc.args[0].priority if exc.args and isinstance(exc.args[0],
                                                                                        Bug) else Bug.PRIORITY.LOW
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
-                        # Format the traceback (Remove unwanted info)
-                        start_res = re.search(r'test_rest_api(.*?)testing(.*?)decorator.py", line (.*?), in inner',
-                                              traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 103:]
+                        # Format the traceback data to remove unwanted info
+                        traceback_data = format_traceback.assert_error(traceback=traceback_data)
                         # Update the test status and details
-                        status, details = TestStatus.FAIL, f'\nTRACEBACKS\n----------\n{traceback_data}'
+                        status, details = TestStatus.FAIL, traceback_data
                     except AttributeError as exc:
-                        # Log the result
-                        test_rest_api_logger.info(
-                            f"{colors.YELLOW}{'ERROR' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
+                        # Log the result to the console
+                        test_rest_api_logger.info(str_color.error(testcase_name))
+                        # Format the exc str to report format
+                        test_rest_api_exc = TestRestApiException(msg=str(exc))
+                        # Update the logs, which has to be added after stdout (eg: error, bug etc)
+                        logs_end = test_rest_api_exc.msg
+                        # Provide a tip for error caused due to await keyword missing scenarios
+                        if "'coroutine' object has no attribute" in logs_end:
+                            logs_end += f'\n\n{"Tip: This may be due to not using await keyword in async Rest api send function calls"}'
                         # Update the error type for reporting
                         error_type = ErrorType.UNEXPECTED
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
-                        # Format the traceback (Remove unwanted info)
-                        start_res = re.search(r'test_rest_api(.*?)testing(.*?)decorator.py", line (.*?), in inner',
-                                              traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 103:]
+                        # Format the traceback data to remove unwanted info
+                        traceback_data = format_traceback.unexpected_exc(traceback=traceback_data)
                         # Update the test status and details
-                        status, details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}\n\n{"Tip: This may be due to not using await keyword in function calls"}'
+                        status, details = TestStatus.ERROR, traceback_data
                     except Exception as exc:
-                        # Log the result
-                        test_rest_api_logger.info(
-                            f"{colors.YELLOW}{'ERROR' : <8}{colors.LIGHT_CYAN}{testcase_name}{colors.LIGHT_BLUE}")
+                        # Log the result to the console
+                        test_rest_api_logger.info(str_color.error(testcase_name))
+                        # Format the exc str to report format
+                        test_rest_api_exc = TestRestApiException(msg=str(exc))
+                        # Update the logs, which has to be added after stdout (eg: error, bug etc)
+                        logs_end = test_rest_api_exc.msg
                         # Update the error type for reporting
                         error_type = ErrorType.UNEXPECTED
                         # Get the code traceback details
                         traceback_data = traceback.format_exc()
-                        # Format the traceback (Remove unwanted info)
-                        start_res = re.search(r'test_rest_api(.*?)testing(.*?)decorator.py", line (.*?), in inner',
-                                              traceback_data)
-                        traceback_data = traceback_data[start_res.start() + 103:]
+                        # Format the traceback data to remove unwanted info
+                        traceback_data = format_traceback.unexpected_exc(traceback=traceback_data)
                         # Update the test status and details
-                        status, details = TestStatus.ERROR, f'\nTRACEBACKS\n----------\n{traceback_data}\n{exc}'
+                        status, details = TestStatus.ERROR, traceback_data
                     finally:
+                        # Set the end time of the test
+                        end = datetime.now().strftime('%Y-%m-%d %H-%M-%S')
+                        # Stop the stopwatch / counter
+                        timer_stop = perf_counter_ns()
+                        # Calculate the time duration of the test in seconds (note: duration is in nanoseconds)
+                        duration = f'{(timer_stop - timer_start) / 1000000000} seconds'
                         # Get standard out messages from all the print() statements
                         stdout_data = string_io.getvalue()
-                        # Update the test logs
-                        logs = f'Started the test\n{stdout_data}'
-                        # Dynamic log msg for different test status
-                        if status == TestStatus.PASS:
-                            logs += 'Completed the test'
-                        elif status == TestStatus.FAIL:
-                            logs += 'Bug!\nTest exited without ending'
-                        elif status == TestStatus.ERROR:
-                            logs += 'Error in code\nTest exited without ending'
-            # Set the end time of the test
-            end = datetime.now().strftime('%Y-%m-%d %H-%M-%S')
-            # Stop the stopwatch / counter
-            timer_stop = perf_counter_ns()
-            # Calculate the time duration of the test in seconds (note: duration is in nanoseconds)
-            duration = f'{(timer_stop - timer_start) / 1000000000} seconds'
+                        # Update the test log's with all the print messages
+                        logs += stdout_data
+                        # Update the end logs for adding details of exception, bug etc.
+                        logs += logs_end
+
             # Create Report test result object instance
             test_result = ReportTestResult(name=testcase_name,
                                            desc=desc,
                                            is_async=is_async,
                                            testsuite=testsuite,
                                            status=status,
                                            details=details,
```

### Comparing `test_rest_api-0.0.0.0.29/test_rest_api/testing/runner.py` & `test_rest_api-0.0.0.0.30/test_rest_api/testing/runner.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import types
 import aiohttp
 import asyncio
 import importlib.machinery
 from datetime import datetime
 from time import perf_counter_ns
 from inspect import getmembers, iscoroutinefunction
-from ..utils.colors import colors
 from ..reporting.report import report
 from ..utils.error_msg import ErrorMsg
+from ..utils.string_color import str_color
 from ..utils.logger import test_rest_api_logger
 from ..utils.aiohttp_session import AioHttpSession
 
 
 class Runner:
     """
     Execute all test cases
@@ -101,80 +101,79 @@
     def setup_testsuite(self):
         """
         Run before test suite execution
         - Load the python files from the input path provided
         - Load all the @test decorated functions from the list of python files
         """
         # Logging
-        test_rest_api_logger.info(f"{colors.WHITE}Starting test setup{colors.LIGHT_BLUE}")
-        test_rest_api_logger.info(f'{colors.WHITE}Auto detecting test suites{colors.LIGHT_BLUE}')
+        test_rest_api_logger.info(str_color.info('Starting test setup'))
+        test_rest_api_logger.info(str_color.info('Auto detecting test suites'))
         # Load python files
         self.load_test_files(self.test_suite_path)
         # Logging
-        test_rest_api_logger.info(f'{colors.WHITE}Total test suites: {len(self.test_files)}{colors.LIGHT_BLUE}')
-        test_rest_api_logger.info(f'{colors.WHITE}Auto detecting tests{colors.LIGHT_BLUE}')
+        test_rest_api_logger.info(str_color.info(f'Total test suites: {len(self.test_files)}'))
+        test_rest_api_logger.info(str_color.info('Auto detecting tests'))
         # Load @test decorated functions from the loaded python files
         self.load_tests()
         # Logging
-        test_rest_api_logger.info(f'{colors.WHITE}Total synchronous tests: {len(self.sync_tests)}{colors.LIGHT_BLUE}')
-        test_rest_api_logger.info(f'{colors.WHITE}Total asynchronous tests: {len(self.async_tests)}{colors.LIGHT_BLUE}')
-        test_rest_api_logger.info(
-            f'{colors.WHITE}Total tests: {len(self.sync_tests) + len(self.async_tests)}{colors.LIGHT_BLUE}')
+        test_rest_api_logger.info(str_color.info(f'Total synchronous tests: {len(self.sync_tests)}'))
+        test_rest_api_logger.info(str_color.info(f'Total asynchronous tests: {len(self.async_tests)}'))
+        test_rest_api_logger.info(str_color.info(f'Total tests: {len(self.sync_tests) + len(self.async_tests)}'))
 
     @staticmethod
     def console_branding():
         """
         Package branding in Console
         """
-        test_rest_api_logger.info(f'''{colors.LIGHT_PURPLE}
+        test_rest_api_logger.info(str_color.brand(f'''
                           =======================================================
                         || ..................................................... ||
                         || ..................................................... ||
                         || ...........  T E S T - R E S T - A P I   ............ ||
                         || ..................................................... ||
                         || ..................................................... ||
                           =======================================================
-                        {colors.LIGHT_BLUE}''')
+                        '''))
 
     @staticmethod
     def console_summary():
         """
         Test Summary in Console
         """
-        test_rest_api_logger.info(f'''{colors.LIGHT_PURPLE}
+        test_rest_api_logger.info(str_color.brand('''
                           =======================================================
                         || ..................................................... ||
                         || ............  T E S T - S U M M A R Y   ............. ||
                         || ..................................................... ||
-                          =======================================================
-                        
-                        {colors.WHITE}{'Status:' : <20}{colors.LIGHT_CYAN}{'PASS' if report.summary.test.status else 'FAIL'}
-                        {colors.WHITE}{'Tests:' : <20}{colors.LIGHT_CYAN}{report.summary.tests.total}
-                        {colors.WHITE}{'Start:' : <20}{colors.LIGHT_CYAN}{report.summary.test.start}
-                        {colors.WHITE}{'End:' : <20}{colors.LIGHT_CYAN}{report.summary.test.end}
-                        {colors.WHITE}{'Duration:' : <20}{colors.LIGHT_CYAN}{report.summary.test.duration}
-                        {colors.WHITE}{'Tags:' : <20}{colors.LIGHT_CYAN}{report.summary.test.tags}
-                        
-                        {colors.WHITE}{'PASS:' : <20}{colors.LIGHT_CYAN}{report.summary.tests.success}
-                        {colors.WHITE}{'FAIL:' : <20}{colors.LIGHT_CYAN}{report.summary.tests.fail}
-                        {colors.WHITE}{'ERROR:' : <20}{colors.LIGHT_CYAN}{report.summary.tests.error}
-                        {colors.WHITE}{'DISABLE:' : <20}{colors.LIGHT_CYAN}{report.summary.tests.disable}
-                        {colors.WHITE}{'SKIP:' : <20}{colors.LIGHT_CYAN}{report.summary.tests.skip}
-                        
-                        {colors.WHITE}{'LOW:' : <20}{colors.LIGHT_CYAN}{report.summary.bugs.low}
-                        {colors.WHITE}{'MINOR:' : <20}{colors.LIGHT_CYAN}{report.summary.bugs.minor}
-                        {colors.WHITE}{'MAJOR:' : <20}{colors.LIGHT_CYAN}{report.summary.bugs.major}
-                        {colors.WHITE}{'CRITICAL:' : <20}{colors.LIGHT_CYAN}{report.summary.bugs.critical}
-                        {colors.WHITE}{'BLOCKER:' : <20}{colors.LIGHT_CYAN}{report.summary.bugs.blocker}
-                        
-                        {colors.WHITE}{'REST API:' : <20}{colors.LIGHT_CYAN}{report.summary.errors.rest_api}
-                        {colors.WHITE}{'GLOBAL VARIABLES:' : <20}{colors.LIGHT_CYAN}{report.summary.errors.global_variables}
-                        {colors.WHITE}{'BUG:' : <20}{colors.LIGHT_CYAN}{report.summary.errors.bug}
-                        {colors.WHITE}{'LOGGER:' : <20}{colors.LIGHT_CYAN}{report.summary.errors.logger}
-                        {colors.WHITE}{'UNEXPECTED:' : <20}{colors.LIGHT_CYAN}{report.summary.errors.unexpected}''')
+                          ======================================================='''))
+        test_rest_api_logger.info(str_color.info(f'''
+                         {'Status:' : <20}{'PASS' if report.summary.test.status else 'FAIL'}
+                         {'Tests:' : <20}{report.summary.tests.total}
+                         {'Start:' : <20}{report.summary.test.start}
+                         {'End:' : <20}{report.summary.test.end}
+                         {'Duration:' : <20}{report.summary.test.duration}
+                         {'Tags:' : <20}{report.summary.test.tags}
+                         
+                         {'PASS:' : <20}{report.summary.tests.success}
+                         {'FAIL:' : <20}{report.summary.tests.fail}
+                         {'ERROR:' : <20}{report.summary.tests.error}
+                         {'DISABLE:' : <20}{report.summary.tests.disable}
+                         {'SKIP:' : <20}{report.summary.tests.skip}
+                         
+                         {'LOW:' : <20}{report.summary.bugs.low}
+                         {'MINOR:' : <20}{report.summary.bugs.minor}
+                         {'MAJOR:' : <20}{report.summary.bugs.major}
+                         {'CRITICAL:' : <20}{report.summary.bugs.critical}
+                         {'BLOCKER:' : <20}{report.summary.bugs.blocker}
+                         
+                         {'REST API:' : <20}{report.summary.errors.rest_api}
+                         {'GLOBAL VARIABLES:' : <20}{report.summary.errors.global_variables}
+                         {'BUG:' : <20}{report.summary.errors.bug}
+                         {'ASSERTION:' : <20}{report.summary.errors.assertion}
+                         {'UNEXPECTED:' : <20}{report.summary.errors.unexpected}'''))
 
     def create_test_report(self):
         """
         Create and save the test report
         """
         # Create the report
         report.save(path=self.test_result_path)
@@ -194,34 +193,34 @@
         self.sync_tests.sort(key=lambda x: x.execution_order)
         # Session should be created inside async function even if it itself not an async function
         # Also creation should happen inside the main event loop (Should not be in a separate event loop)
         session = aiohttp.ClientSession(json_serialize=json.dumps)
         # Create an aiohttp session for the whole run instead of creating a new session per request.
         AioHttpSession.set(session=session)
         # Logging
-        test_rest_api_logger.info(f"{colors.WHITE}Created aiohttp client session{colors.LIGHT_BLUE}")
-        test_rest_api_logger.info(f"{colors.WHITE}Completed test setup{colors.LIGHT_BLUE}")
+        test_rest_api_logger.info(str_color.info('Created aiohttp client session'))
+        test_rest_api_logger.info(str_color.info('Completed test setup'))
         if len(self.sync_tests) > 0:
-            test_rest_api_logger.info(f"""{colors.LIGHT_PURPLE}
+            test_rest_api_logger.info(str_color.brand("""
                           =======================================================
                         || ................  S Y N C - T E S T S ............... ||
-                          ======================================================={colors.LIGHT_BLUE}""")
+                          ======================================================="""))
         # Start the stopwatch / counter
         timer_start = perf_counter_ns()
         # Test start date time
         start = datetime.now().strftime('%Y-%m-%d %H-%M-%S')
         # Run synchronous tests before async tests
         for sync_test in (sync_test for sync_test in self.sync_tests):
             await sync_test()
         # Logging
         if len(self.async_tests) > 0:
-            test_rest_api_logger.info(f"""{colors.LIGHT_PURPLE}
+            test_rest_api_logger.info(str_color.brand("""
                           =======================================================
                         || ............... A S Y N C - T E S T S ............... ||
-                          ======================================================={colors.LIGHT_BLUE}""")
+                          ======================================================="""))
         # Running Tasks Concurrently (Execute async functions concurrently)
         # Run all async functions from tests list in parallel
         await asyncio.gather(*[async_test() for async_test in self.async_tests], return_exceptions=False)
         # Test end time
         end = datetime.now().strftime('%Y-%m-%d %H-%M-%S')
         # Stop the stopwatch / counter
         timer_stop = perf_counter_ns()
```

### Comparing `test_rest_api-0.0.0.0.29/test_rest_api/utils/aiohttp_session.py` & `test_rest_api-0.0.0.0.30/test_rest_api/utils/aiohttp_session.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.29/test_rest_api/utils/logger.py` & `test_rest_api-0.0.0.0.30/test_rest_api/utils/logger.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.29/test_rest_api.egg-info/PKG-INFO` & `test_rest_api-0.0.0.0.30/test_rest_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-rest-api
-Version: 0.0.0.0.29
+Version: 0.0.0.0.30
 Summary: Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests
 Home-page: https://github.com/troymjose/test_rest_api
 Author: Troy M Jose
 Author-email: 
 Project-URL: Source, https://github.com/troymjose/test_rest_api
 Project-URL: Tracker, https://github.com/troymjose/test_rest_api/issues
 Keywords: test,unittest,restapi,testframework,asyncio,async,asynchronous,testingframework,rest,api,python,python3,testing,unittesting,automation,automationtest,automationtesting,restapitest,restapitesting,restapiunittest,restapiunittesting,restapiautomation,restapiautomationtest,restapiautomationtesting,apitest,apitesting,apiunittest,apiunittesting,apiautomation,apiautomationtest,apiautomationtesting
@@ -44,26 +44,27 @@
     - [Set report path](#2-set-report-path)
     - [Set .env path](#3-set-env-path)
     - [Set hashtags](#4-set-hashtags)
     - [Project structure](#5-project-structure)
 - [Examples](#examples)
     - [My first test](#1-my-first-test)
     - [Configure my test](#2-configure-my-test)
-    - [My first logger](#3-my-first-logger)
-    - [Set global variables value](#4-set-global-variables-value)
-    - [Set global variables value as constant](#5-set-global-variables-value-as-constant)
-    - [Get global variables value](#6-get-global-variables-value)
-    - [My first bug](#7-my-first-bug)
-    - [Configure my bug](#8-configure-my-bug)
-    - [My first rest api](#9-my-first-rest-api)
-    - [Configure my rest api](#10-configure-my-rest-api)
-    - [Reuse my rest api](#11-reuse-my-rest-api)
-    - [Send my rest api](#12-send-my-rest-api)
-    - [Rest api response](#13-rest-api-response)
-    - [Demo with all the above features](#14-demo)
+    - [Replace inbuilt assert](#3-replace-inbuilt-assert)
+    - [My first log](#4-my-first-log)
+    - [Set global variables value](#5-set-global-variables-value)
+    - [Set global variables value as constant](#6-set-global-variables-value-as-constant)
+    - [Get global variables value](#7-get-global-variables-value)
+    - [My first bug](#8-my-first-bug)
+    - [Configure my bug](#9-configure-my-bug)
+    - [My first rest api](#10-my-first-rest-api)
+    - [Configure my rest api](#11-configure-my-rest-api)
+    - [Reuse my rest api](#12-reuse-my-rest-api)
+    - [Send my rest api](#13-send-my-rest-api)
+    - [Rest api response](#14-rest-api-response)
+    - [Demo with all the above features](#15-demo)
 - [Reports](#reports)
     - [My first report](#1-my-first-report)
     - [Async tests report](#2-async-tests-report)
     - [Sync tests report](#3-sync-tests-report)
     - [Sync & Async report](#4-sync-and-async-report)
     - [Multi status report](#5-multi-status-report)
     - [Multi bug report](#6-multi-bug-report)
@@ -206,15 +207,15 @@
 
 ```python
 from test_rest_api import test
 
 
 @test()
 async def my_first_test():
-    return None
+    assert 4 == 5
 ```   
 
 - Create an __async__ python function with any __custom__ name
 - Decorate the function using __@test()__
 - __Async__ python functions decoratd with __@test()__ will be auto-detected as testcase
 - __Normal__ python functions decoratd with __@test()__ will __not__ be considered as testcase
 
@@ -238,15 +239,15 @@
 
 ```python
 from test_rest_api import test
 
 
 @test(name='Custom Name', desc='Description', enabled=True, tags=['SMOKE', 'ABC'], is_async=True, execution_order='1')
 async def my_second_test():
-    return None
+    assert 4 == 5
 ```
 
 - In our first example, we used @test() decorator with __empty parameters__
 - In this example, we are __using parameters__ to configure our test function
 - This can be considered as adding __settings__ to your test function
 
 
@@ -277,38 +278,55 @@
     - Default: True
 - __execution_order__
     - Mandatory: False
     - Data Type: str
     - Expected: Custom text for ordering. This will work only when is_async = False
     - Default: 'zzzzz'
 
-<h4 id="3-my-first-logger">3. My first logger</h4>
+<h4 id="3-replace-inbuilt-assert">3. Replace inbuilt assert</h4>
 
 - - -
 
 ```python
-from test_rest_api import test, Logger
+from test_rest_api import test, Assert
 
 
 @test()
 async def my_first_logger():
-    logger = Logger()
-    logger.log("my 1st log")
-    logger.log("my 2nd log")
-    return logger 
+    # assert 4 == 5
+    Assert.equal(4, 5)
+```
+
+- Assert is same as inbuilt python assert statement
+- Using test rest api Assert class improves logging
+- Assertions done using Assert will be automatically logged in final html report
+- It is __recommended__ to use Assert instead of inbuilt assert statement for all your tests
+
+<h4 id="4-my-first-log">4. My first log</h4>
+
+- - -
+
+```python
+from test_rest_api import test
+
+
+@test()
+async def my_first_logger():
+    print('My 1st log')
+    print('My 2nd log')
+    assert 4 == 5
 ```
 
-- Loggers are used to add __custom messages__ to the final html test report
-- Create a new Logger __instance__ inside your test function```logger = Logger()```
-- Logger instance __name__ can be any custom text. Here we have used __logger__
-- Add any number of log messages using __log method__ ```logger.log("my 1st log")```
-- Return logger instance for rich test __reporting__ ```return logger```
-- It is __recommended__ to use logger for all your tests
+- Python inbuilt ```print()``` function is used to add __custom messages__ to the final html test report
+- Add print() functions inside your __test function__
+- Add any number of log messages without any limit
+- It is __recommended__ to add logs for all your tests
+- Note: ```print()``` statements will not be printed to console
 
-<h4 id="4-set-global-variables-value">4. Set global variables value</h4>
+<h4 id="5-set-global-variables-value">5. Set global variables value</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, GlobalVariables
 
 
@@ -330,15 +348,15 @@
     - Data Type: str
     - Expected: Custom name for your global variable
 - __value__
     - Mandatory: True
     - Data Type: any
     - Expected: Any python data type can be stored as global variables value
 
-<h4 id="5-set-global-variables-value-as-constant">5. Set global variables value as constant</h4>
+<h4 id="6-set-global-variables-value-as-constant">6. Set global variables value as constant</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, GlobalVariables
 
 
@@ -365,15 +383,15 @@
     - Expected: Any python data type can be stored as global variables value
 - __is_constant__
     - Mandatory: False
     - Data Type: bool
     - Expected: True or False. Provide True, to create constants
     - Default: False
 
-<h4 id="6-get-global-variables-value">6. Get global variables value</h4>
+<h4 id="7-get-global-variables-value">7. Get global variables value</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, GlobalVariables
 
 
@@ -391,15 +409,15 @@
 ```GlobalVariables.get(name='token')```
 
 - __name__
     - Mandatory: True
     - Data Type: str
     - Expected: Valid name of any saved global variable
 
-<h4 id="7-my-first-bug">7. My first bug</h4>
+<h4 id="8-my-first-bug">8. My first bug</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, Bug
 
 
@@ -410,15 +428,15 @@
 
 - Bug is used to __raise issues__ in tests
 - Add custom __checks__ in your tests to validate __rest api response__
 - If __actual result__ is not the __expected result__, just call ```Bug()```
 - This will __terminate__ the current test function execution
 - Bug __details__ can be viewed in final html test __report__
 
-<h4 id="8-configure-my-bug">8. Configure my bug</h4>
+<h4 id="9-configure-my-bug">9. Configure my bug</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, Bug, Logger
 
 
@@ -463,15 +481,15 @@
     - Default: Empty list
 - __steps_to_reproduce__
     - Mandatory: False
     - Data Type: str
     - Expected: Logger instance can be used to auto-populate this field
     - Default: Empty string
 
-<h4 id="9-my-first-rest-api">9. My first rest api</h4>
+<h4 id="10-my-first-rest-api">10. My first rest api</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, RestApi
 
 
@@ -481,15 +499,15 @@
 ```
 
 - RestApi is used __create__ rest api instance in tests
 - Here we have created a basic rest api with just the __url information__
 - This example is only about creating rest api, no __send action__ is performed here
 - We will use this __instance variable__ for sending the request in upcoming examples
 
-<h4 id="10-configure-my-rest-api">10. Configure my rest api</h4>
+<h4 id="11-configure-my-rest-api">11. Configure my rest api</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, RestApi
 
 
@@ -519,15 +537,15 @@
     - Default: {}
 - __body__
     - Mandatory: False
     - Data Type: dict
     - Expected: Provide the json request payload
     - Default: {}
 
-<h4 id="11-reuse-my-rest-api">11. Reuse my rest api</h4>
+<h4 id="12-reuse-my-rest-api">12. Reuse my rest api</h4>
 
 - - -
 
 ```python
 from test_rest_api import RestApi, GlobalVariables
 
 
@@ -547,15 +565,15 @@
 - Use python __functions__ to create a rest api which will avoid __code duplication__
 - You can __call__ a function __100__ times instead of __writing__ it __100__ times
 - In this example we have created a simple __login api__
 - All the __dynamic values__ for rest api creation can be passed as function __parameters__
 - This helps in calling the same api with __different inputs__
 - Return the __RestApi instance__ which can be used in test functions for __sending__
 
-<h4 id="12-send-my-rest-api">12. Send my rest api</h4>
+<h4 id="13-send-my-rest-api">13. Send my rest api</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, RestApi
 
 
@@ -571,15 +589,15 @@
 - Now it's time to __send__ them using http methods
 - __Supported__ http methods are GET, POST, PUT, PATCH, DELETE, OPTIONS & HEAD
 - Here we are sending the rest_api using __GET__ http method
 - All the responses (1, 2 & 3) will have the __same result__
 - Because they perform the same functionality with __different syntax__
 - Similarly, __other http methods__ can be used, with your desired syntax
 
-<h4 id="13-rest-api-response">13. Rest api response</h4>
+<h4 id="14-rest-api-response">14. Rest api response</h4>
 
 - - -
 
 ```python
 from test_rest_api import test, RestApi
 
 
@@ -613,15 +631,15 @@
 - __response.content_type__
     - Data Type: str
     - Value: Response content type
 - __response.obj__
     - Data Type: aiohttp.ClientResponse
     - Value: Python aiohttp ClientResponse object
 
-<h4 id="14-demo">14. Demo with all the above features</h4>
+<h4 id="15-demo">15. Demo with all the above features</h4>
 
 - - -
 
 ```
 .env file
 ---------
```

### Comparing `test_rest_api-0.0.0.0.29/test_rest_api.egg-info/SOURCES.txt` & `test_rest_api-0.0.0.0.30/test_rest_api.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,31 +4,37 @@
 test_rest_api/__init__.py
 test_rest_api/__main__.py
 test_rest_api.egg-info/PKG-INFO
 test_rest_api.egg-info/SOURCES.txt
 test_rest_api.egg-info/dependency_links.txt
 test_rest_api.egg-info/requires.txt
 test_rest_api.egg-info/top_level.txt
+test_rest_api/assertion/__init__.py
+test_rest_api/assertion/assertion.py
+test_rest_api/assertion/exception.py
 test_rest_api/global_variables/__init__.py
 test_rest_api/global_variables/exception.py
 test_rest_api/global_variables/global_variables.py
 test_rest_api/reporting/__init__.py
 test_rest_api/reporting/html.py
 test_rest_api/reporting/report.py
 test_rest_api/rest_api/__init__.py
-test_rest_api/rest_api/dot_dict.py
 test_rest_api/rest_api/exception.py
 test_rest_api/rest_api/method.py
 test_rest_api/rest_api/response.py
 test_rest_api/rest_api/rest_api.py
+test_rest_api/settings/__init__.py
+test_rest_api/settings/logging.py
 test_rest_api/testing/__init__.py
 test_rest_api/testing/bug.py
 test_rest_api/testing/decorator.py
 test_rest_api/testing/exception.py
 test_rest_api/testing/runner.py
+test_rest_api/testing/traceback.py
+test_rest_api/testing/utils.py
 test_rest_api/utils/__init__.py
 test_rest_api/utils/aiohttp_session.py
-test_rest_api/utils/colors.py
 test_rest_api/utils/decorator_hints.py
 test_rest_api/utils/error_msg.py
 test_rest_api/utils/exception.py
-test_rest_api/utils/logger.py
+test_rest_api/utils/logger.py
+test_rest_api/utils/string_color.py
```

