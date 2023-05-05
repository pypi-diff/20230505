# Comparing `tmp/volworld_aws_api_common-0.1.91.tar.gz` & `tmp/volworld_aws_api_common-0.1.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volworld_aws_api_common-0.1.91.tar", last modified: Wed May  3 08:06:53 2023, max compression
+gzip compressed data, was "volworld_aws_api_common-0.1.92.tar", last modified: Fri May  5 03:28:26 2023, max compression
```

## Comparing `volworld_aws_api_common-0.1.91.tar` & `volworld_aws_api_common-0.1.92.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 08:06:53.013155 volworld_aws_api_common-0.1.91/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1070 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/LICENSE.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      251 2023-05-03 08:06:53.013155 volworld_aws_api_common-0.1.91/PKG-INFO
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       31 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/README.rst
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       38 2023-05-03 08:06:53.013155 volworld_aws_api_common-0.1.91/setup.cfg
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      387 2023-05-03 08:06:51.000000 volworld_aws_api_common-0.1.91/setup.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 08:06:53.009155 volworld_aws_api_common-0.1.91/src/
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 08:06:53.009155 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 08:06:53.013155 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/api/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      158 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/api/AA.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       76 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/api/Aws.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      222 2023-05-03 00:54:51.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/api/Url.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/api/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 08:06:53.013155 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/api/enum/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      200 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/api/enum/ErrorCode.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      859 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/api/enum/HttpStatus.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       99 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/api/enum/ProjectModeType.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      116 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/api/enum/QueryModeType.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/api/enum/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 08:06:53.013155 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/api/url/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/api/url/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      787 2023-05-03 07:56:29.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/api/url/authUrl.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 08:06:53.013155 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      156 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/ProjectMode.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      150 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/QueryMode.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     3403 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/UserPool.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 08:06:53.013155 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/api/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      424 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/api/OAPI.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     3049 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/api/OpenApiValidation.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/api/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     2499 2023-05-03 08:06:44.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/api/request_open_api_validation.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 08:06:53.013155 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/aws/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      146 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/aws/ATestRequest.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/aws/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 08:06:53.013155 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/aws/request/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/aws/request/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1009 2023-05-03 07:57:11.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/aws/request/get__current_user.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1557 2023-05-03 07:56:55.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/aws/request/post__login.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1303 2023-05-03 07:57:02.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/aws/request/post__signup.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      547 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/aws/request/request_util.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      669 2023-05-03 04:56:52.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/aws/url.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 08:06:53.013155 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/behave/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      118 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/behave/ACotA.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/behave/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     4729 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/request.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 08:06:53.009155 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common.egg-info/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      251 2023-05-03 08:06:52.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common.egg-info/PKG-INFO
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1840 2023-05-03 08:06:52.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common.egg-info/SOURCES.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        1 2023-05-03 08:06:52.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common.egg-info/dependency_links.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       22 2023-05-03 08:06:52.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common.egg-info/requires.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       24 2023-05-03 08:06:52.000000 volworld_aws_api_common-0.1.91/src/volworld_aws_api_common.egg-info/top_level.txt
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:28:26.399689 volworld_aws_api_common-0.1.92/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1070 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/LICENSE.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      199 2023-05-05 03:28:26.399689 volworld_aws_api_common-0.1.92/PKG-INFO
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       31 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/README.rst
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       38 2023-05-05 03:28:26.399689 volworld_aws_api_common-0.1.92/setup.cfg
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      387 2023-05-05 03:28:24.000000 volworld_aws_api_common-0.1.92/setup.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:28:26.363689 volworld_aws_api_common-0.1.92/src/
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:28:26.395689 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:28:26.395689 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/api/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      158 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/api/AA.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       76 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/api/Aws.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      222 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/api/Url.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/api/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:28:26.395689 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/api/enum/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      200 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/api/enum/ErrorCode.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      859 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/api/enum/HttpStatus.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       99 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/api/enum/ProjectModeType.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      116 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/api/enum/QueryModeType.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/api/enum/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:28:26.395689 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/api/url/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/api/url/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      809 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/api/url/authUrl.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:28:26.395689 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      156 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/ProjectMode.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      150 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/QueryMode.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     3403 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/UserPool.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:28:26.399689 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/api/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      424 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/api/OAPI.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     3049 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/api/OpenApiValidation.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/api/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     2499 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/api/request_open_api_validation.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:28:26.399689 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/aws/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      146 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/aws/ATestRequest.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/aws/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:28:26.399689 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/aws/request/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/aws/request/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1009 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/aws/request/get__current_user.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1557 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/aws/request/post__login.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1303 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/aws/request/post__signup.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      547 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/aws/request/request_util.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      669 2023-05-05 03:26:25.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/aws/url.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:28:26.399689 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/behave/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      118 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/behave/ACotA.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/behave/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     4729 2023-05-05 03:25:57.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/request.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-05 03:28:26.395689 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common.egg-info/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      199 2023-05-05 03:28:26.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common.egg-info/PKG-INFO
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1840 2023-05-05 03:28:26.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        1 2023-05-05 03:28:26.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       22 2023-05-05 03:28:26.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common.egg-info/requires.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       24 2023-05-05 03:28:26.000000 volworld_aws_api_common-0.1.92/src/volworld_aws_api_common.egg-info/top_level.txt
```

### Comparing `volworld_aws_api_common-0.1.91/LICENSE.txt` & `volworld_aws_api_common-0.1.92/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/api/enum/HttpStatus.py` & `volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/api/enum/HttpStatus.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/api/url/authUrl.py` & `volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/api/url/authUrl.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # doLoginUrl: Final[str] = build_url(ROOT__, AA.Login)
 #
 # # doLogoutUrl: Final[str] = build_url(ROOT__, AA.Logout)
 #
 # currentUserUrl: Final[str] = build_url(ROOT__, AA.UserId)
 
 
-
+ROOT__: Final[list] = [AA.Auth]
 
 def do_signup_url():
-    return build_dynamic_url([AA.Auth], [AA.Signup])
+    return build_dynamic_url(ROOT__, [AA.Signup])
 
 def do_login_url():
-    return build_dynamic_url([AA.Auth], [AA.Login])
+    return build_dynamic_url(ROOT__, [AA.Login])
 
 def current_user_url():
-    return build_dynamic_url([AA.Auth], [AA.UserId])
+    return build_dynamic_url(ROOT__, [AA.UserId])
```

### Comparing `volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/UserPool.py` & `volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/UserPool.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/api/OpenApiValidation.py` & `volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/api/OpenApiValidation.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/api/request_open_api_validation.py` & `volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/api/request_open_api_validation.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/aws/request/get__current_user.py` & `volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/aws/request/get__current_user.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/aws/request/post__login.py` & `volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/aws/request/post__login.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/aws/request/post__signup.py` & `volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/aws/request/post__signup.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/aws/request/request_util.py` & `volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/aws/request/request_util.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/aws/url.py` & `volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/aws/url.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,8 @@
         es.append(e)
     return f"{root}/{'/'.join(es)}"
     # return root + '/' + '/'.join(es)
 
 
 def build_dynamic_url(root: list, path: list):
     root = f"{Url.Root}{AA.Api}/{'/'.join(root)}"
-    return f"{root}/{'/'.join(path)}"
+    return f"{root}/{'-'.join(path)}"
```

### Comparing `volworld_aws_api_common-0.1.91/src/volworld_aws_api_common/test/request.py` & `volworld_aws_api_common-0.1.92/src/volworld_aws_api_common/test/request.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.91/src/volworld_aws_api_common.egg-info/SOURCES.txt` & `volworld_aws_api_common-0.1.92/src/volworld_aws_api_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

