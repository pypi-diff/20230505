# Comparing `tmp/volworld_aws_api_common-0.1.94.tar.gz` & `tmp/volworld_aws_api_common-0.1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volworld_aws_api_common-0.1.94.tar", last modified: Fri May  5 12:51:15 2023, max compression
+gzip compressed data, was "volworld_aws_api_common-0.1.95.tar", last modified: Fri May  5 12:52:44 2023, max compression
```

## Comparing `volworld_aws_api_common-0.1.94.tar` & `volworld_aws_api_common-0.1.95.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:51:15.296672 volworld_aws_api_common-0.1.94/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1070 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/LICENSE.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      199 2023-05-05 12:51:15.292672 volworld_aws_api_common-0.1.94/PKG-INFO
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       31 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/README.rst
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       38 2023-05-05 12:51:15.296672 volworld_aws_api_common-0.1.94/setup.cfg
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      387 2023-05-05 12:51:12.000000 volworld_aws_api_common-0.1.94/setup.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:51:15.120669 volworld_aws_api_common-0.1.94/src/
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:51:15.252671 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:51:15.252671 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/api/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      158 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/api/AA.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       76 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/api/Aws.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      222 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/api/Url.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/api/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:51:15.256671 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/api/enum/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      200 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/api/enum/ErrorCode.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      859 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/api/enum/HttpStatus.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       99 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/api/enum/ProjectModeType.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      116 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/api/enum/QueryModeType.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/api/enum/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:51:15.256671 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/api/url/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/api/url/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      809 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/api/url/authUrl.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:51:15.256671 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      156 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/ProjectMode.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      150 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/QueryMode.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     3403 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/UserPool.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:51:15.256671 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/api/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      424 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/api/OAPI.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     3049 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/api/OpenApiValidation.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/api/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     3149 2023-05-05 12:51:06.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/api/request_open_api_validation.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:51:15.260671 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/aws/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      146 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/aws/ATestRequest.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/aws/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:51:15.292672 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/aws/request/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/aws/request/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1009 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/aws/request/get__current_user.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1557 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/aws/request/post__login.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1303 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/aws/request/post__signup.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      547 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/aws/request/request_util.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      669 2023-05-05 03:26:25.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/aws/url.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:51:15.292672 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/behave/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      118 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/behave/ACotA.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/behave/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     4729 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/request.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:51:15.252671 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common.egg-info/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      199 2023-05-05 12:51:14.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common.egg-info/PKG-INFO
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1840 2023-05-05 12:51:15.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common.egg-info/SOURCES.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        1 2023-05-05 12:51:15.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common.egg-info/dependency_links.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       22 2023-05-05 12:51:15.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common.egg-info/requires.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       24 2023-05-05 12:51:15.000000 volworld_aws_api_common-0.1.94/src/volworld_aws_api_common.egg-info/top_level.txt
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.870172 volworld_aws_api_common-0.1.95/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1070 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/LICENSE.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      199 2023-05-05 12:52:44.866172 volworld_aws_api_common-0.1.95/PKG-INFO
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       31 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/README.rst
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       38 2023-05-05 12:52:44.870172 volworld_aws_api_common-0.1.95/setup.cfg
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      387 2023-05-05 12:52:42.000000 volworld_aws_api_common-0.1.95/setup.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.758170 volworld_aws_api_common-0.1.95/src/
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.862172 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.862172 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      158 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/AA.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       76 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/Aws.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      222 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/Url.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.866172 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/enum/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      200 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/enum/ErrorCode.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      859 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/enum/HttpStatus.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       99 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/enum/ProjectModeType.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      116 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/enum/QueryModeType.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/enum/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.866172 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/url/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/url/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      809 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/url/authUrl.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.866172 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      156 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/ProjectMode.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      150 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/QueryMode.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     3403 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/UserPool.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.866172 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/api/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      424 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/api/OAPI.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     3049 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/api/OpenApiValidation.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/api/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     3143 2023-05-05 12:52:37.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/api/request_open_api_validation.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.866172 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      146 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/ATestRequest.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.866172 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/request/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/request/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1009 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/request/get__current_user.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1557 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/request/post__login.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1303 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/request/post__signup.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      547 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/request/request_util.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      669 2023-05-05 03:26:25.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/url.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.866172 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/behave/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      118 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/behave/ACotA.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/behave/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     4729 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/request.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 12:52:44.862172 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common.egg-info/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      199 2023-05-05 12:52:44.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common.egg-info/PKG-INFO
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1840 2023-05-05 12:52:44.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        1 2023-05-05 12:52:44.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       22 2023-05-05 12:52:44.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common.egg-info/requires.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       24 2023-05-05 12:52:44.000000 volworld_aws_api_common-0.1.95/src/volworld_aws_api_common.egg-info/top_level.txt
```

### Comparing `volworld_aws_api_common-0.1.94/LICENSE.txt` & `volworld_aws_api_common-0.1.95/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/api/enum/HttpStatus.py` & `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/enum/HttpStatus.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/api/url/authUrl.py` & `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/api/url/authUrl.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/UserPool.py` & `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/UserPool.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/api/OpenApiValidation.py` & `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/api/OpenApiValidation.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/api/request_open_api_validation.py` & `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/api/request_open_api_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     print("[db_fn_open_api_validation] res = ", resp_json)
     print("[db_fn_open_api_validation] resp.status_code = ", resp.status_code)
     if AA.___Error___ not in resp_json:
         if 'message' in resp_json:
             if resp_json['message'] == 'Invalid request body':
                 val.validate_GET_response({
-                    AA.___Error___: resp_json[AA.___Error___]
+                    AA.___Error___: 'Invalid request body'
                 }, url, ErrorCode.WrongUserNameFormat.value, attList)
                 return
         val.validate_POST_response({
             AA.Data: resp_json[AA.Data]
         }, url, resp.status_code, attList)
     else:
         val.validate_POST_response({
@@ -45,15 +45,15 @@
 
     print("[db_fn_open_api_validation] res = ", resp_json)
     print("[db_fn_open_api_validation] resp.status_code = ", resp.status_code)
     if AA.___Error___ not in resp_json:
         if 'message' in resp_json:
             if resp_json['message'] == 'Invalid request body':
                 val.validate_GET_response({
-                    AA.___Error___: resp_json[AA.___Error___]
+                    AA.___Error___: 'Invalid request body'
                 }, url, ErrorCode.WrongUserNameFormat.value, attList)
                 return
         val.validate_GET_response({
             AA.Data: resp_json[AA.Data]
         }, url, resp.status_code, attList)
     else:
         val.validate_GET_response({
```

### Comparing `volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/aws/request/get__current_user.py` & `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/request/get__current_user.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/aws/request/post__login.py` & `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/request/post__login.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/aws/request/post__signup.py` & `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/request/post__signup.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/aws/request/request_util.py` & `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/request/request_util.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/aws/url.py` & `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/aws/url.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.94/src/volworld_aws_api_common/test/request.py` & `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common/test/request.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.94/src/volworld_aws_api_common.egg-info/SOURCES.txt` & `volworld_aws_api_common-0.1.95/src/volworld_aws_api_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

