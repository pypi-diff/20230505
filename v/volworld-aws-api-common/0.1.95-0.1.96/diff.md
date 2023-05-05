# Comparing `tmp/volworld_aws_api_common-0.1.95.tar.gz` & `tmp/volworld_aws_api_common-0.1.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volworld_aws_api_common-0.1.95.tar", last modified: Fri May  5 12:52:44 2023, max compression
+gzip compressed data, was "volworld_aws_api_common-0.1.96.tar", last modified: Fri May  5 12:55:11 2023, max compression
```

## Comparing `volworld_aws_api_common-0.1.95.tar` & `volworld_aws_api_common-0.1.96.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.870172 volworld_aws_api_common-0.1.95/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1070 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/LICENSE.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      199 2023-05-05 12:52:44.866172 volworld_aws_api_common-0.1.95/PKG-INFO
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       31 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/README.rst
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       38 2023-05-05 12:52:44.870172 volworld_aws_api_common-0.1.95/setup.cfg
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      387 2023-05-05 12:52:42.000000 volworld_aws_api_common-0.1.95/setup.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.758170 volworld_aws_api_common-0.1.95/src/
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.862172 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.862172 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      158 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/AA.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       76 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/Aws.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      222 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/Url.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.866172 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/enum/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      200 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/enum/ErrorCode.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      859 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/enum/HttpStatus.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       99 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/enum/ProjectModeType.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      116 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/enum/QueryModeType.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/enum/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.866172 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/url/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/url/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      809 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/url/authUrl.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.866172 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      156 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/ProjectMode.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      150 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/QueryMode.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     3403 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/UserPool.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.866172 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/api/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      424 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/api/OAPI.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     3049 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/api/OpenApiValidation.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/api/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     3143 2023-05-05 12:52:37.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/api/request_open_api_validation.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.866172 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      146 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/ATestRequest.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.866172 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/request/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/request/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1009 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/request/get__current_user.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1557 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/request/post__login.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1303 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/request/post__signup.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      547 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/request/request_util.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      669 2023-05-05 03:26:25.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/url.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.866172 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/behave/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      118 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/behave/ACotA.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/behave/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     4729 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/request.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.862172 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common.egg-info/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      199 2023-05-05 12:52:44.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common.egg-info/PKG-INFO
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1840 2023-05-05 12:52:44.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common.egg-info/SOURCES.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        1 2023-05-05 12:52:44.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common.egg-info/dependency_links.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       22 2023-05-05 12:52:44.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common.egg-info/requires.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       24 2023-05-05 12:52:44.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common.egg-info/top_level.txt
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:55:11.752611 volworld_aws_api_common-0.1.96/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1070 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/LICENSE.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      199 2023-05-05 12:55:11.752611 volworld_aws_api_common-0.1.96/PKG-INFO
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       31 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/README.rst
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       38 2023-05-05 12:55:11.752611 volworld_aws_api_common-0.1.96/setup.cfg
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      387 2023-05-05 12:55:09.000000 volworld_aws_api_common-0.1.96/setup.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:55:11.500607 volworld_aws_api_common-0.1.96/src/
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:55:11.744611 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:55:11.748611 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/api/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      158 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/api/AA.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       76 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/api/Aws.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      222 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/api/Url.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/api/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:55:11.748611 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/api/enum/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      231 2023-05-05 12:54:46.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/api/enum/ErrorCode.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      859 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/api/enum/HttpStatus.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       99 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/api/enum/ProjectModeType.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      116 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/api/enum/QueryModeType.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/api/enum/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:55:11.748611 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/api/url/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/api/url/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      809 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/api/url/authUrl.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:55:11.748611 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      156 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/ProjectMode.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      150 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/QueryMode.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     3403 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/UserPool.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:55:11.748611 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/api/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      424 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/api/OAPI.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     3049 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/api/OpenApiValidation.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/api/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     3208 2023-05-05 12:55:05.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/api/request_open_api_validation.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:55:11.752611 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/aws/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      146 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/aws/ATestRequest.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/aws/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:55:11.752611 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/aws/request/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/aws/request/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1009 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/aws/request/get__current_user.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1557 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/aws/request/post__login.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1303 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/aws/request/post__signup.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      547 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/aws/request/request_util.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      669 2023-05-05 03:26:25.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/aws/url.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:55:11.752611 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/behave/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      118 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/behave/ACotA.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/behave/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     4729 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/request.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:55:11.744611 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common.egg-info/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      199 2023-05-05 12:55:11.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common.egg-info/PKG-INFO
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1840 2023-05-05 12:55:11.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        1 2023-05-05 12:55:11.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       22 2023-05-05 12:55:11.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common.egg-info/requires.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       24 2023-05-05 12:55:11.000000 volworld_aws_api_common-0.1.96/src/volworld_aws_api_common.egg-info/top_level.txt
```

### Comparing `volworld_aws_api_common-0.1.95/LICENSE.txt` & `volworld_aws_api_common-0.1.96/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/enum/HttpStatus.py` & `volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/api/enum/HttpStatus.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/url/authUrl.py` & `volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/api/url/authUrl.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/UserPool.py` & `volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/UserPool.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/api/OpenApiValidation.py` & `volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/api/OpenApiValidation.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/api/request_open_api_validation.py` & `volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/api/request_open_api_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from requests import Response
 from volworld_common.test.Timer import Timer
 from volworld_aws_api_common.api.AA import AA
 from volworld_aws_api_common.api.Url import Url
 from volworld_aws_api_common.test.aws.ATestRequest import ATestRequest
 from volworld_aws_api_common.test.request import post_request, get_request
+from volworld_aws_api_common.api.enum.ErrorCode import ErrorCode
 
 from volworld_aws_api_common.test.api.OpenApiValidation import OpenApiValidation
 
 
 def request_open_api_post_validation(url: str, req, resp_json, resp: Response, attList):
     url = url.replace(Url.Root, '')
     url = url.replace('//', '/')
```

### Comparing `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/request/get__current_user.py` & `volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/aws/request/get__current_user.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/request/post__login.py` & `volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/aws/request/post__login.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/request/post__signup.py` & `volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/aws/request/post__signup.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/request/request_util.py` & `volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/aws/request/request_util.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/url.py` & `volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/aws/url.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/request.py` & `volworld_aws_api_common-0.1.96/src/volworld_aws_api_common/test/request.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common.egg-info/SOURCES.txt` & `volworld_aws_api_common-0.1.96/src/volworld_aws_api_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

