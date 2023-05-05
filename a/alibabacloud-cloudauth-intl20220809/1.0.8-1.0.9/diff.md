# Comparing `tmp/alibabacloud_cloudauth-intl20220809-1.0.8.tar.gz` & `tmp/alibabacloud_cloudauth-intl20220809-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloudauth-intl20220809-1.0.8.tar", last modified: Wed Apr 19 04:26:21 2023, max compression
+gzip compressed data, was "dist/alibabacloud_cloudauth-intl20220809-1.0.9.tar", last modified: Fri May  5 07:43:51 2023, max compression
```

## Comparing `alibabacloud_cloudauth-intl20220809-1.0.8.tar` & `alibabacloud_cloudauth-intl20220809-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      295 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2394 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1055 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1140 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15320 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809/client.py
--rw-r--r--   0 root         (0) root         (0)    22196 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2394 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      508 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2667 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 07:43:51.000000 alibabacloud_cloudauth-intl20220809-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      338 2023-05-05 07:43:50.000000 alibabacloud_cloudauth-intl20220809-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-05 07:43:50.000000 alibabacloud_cloudauth-intl20220809-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-05 07:43:50.000000 alibabacloud_cloudauth-intl20220809-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-05-05 07:43:51.000000 alibabacloud_cloudauth-intl20220809-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-05-05 07:43:50.000000 alibabacloud_cloudauth-intl20220809-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-05-05 07:43:50.000000 alibabacloud_cloudauth-intl20220809-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 07:43:51.000000 alibabacloud_cloudauth-intl20220809-1.0.9/alibabacloud_cloudauth_intl20220809/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-05 07:43:50.000000 alibabacloud_cloudauth-intl20220809-1.0.9/alibabacloud_cloudauth_intl20220809/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2023-05-05 07:43:50.000000 alibabacloud_cloudauth-intl20220809-1.0.9/alibabacloud_cloudauth_intl20220809/client.py
+-rw-r--r--   0 root         (0) root         (0)    55685 2023-05-05 07:43:50.000000 alibabacloud_cloudauth-intl20220809-1.0.9/alibabacloud_cloudauth_intl20220809/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 07:43:51.000000 alibabacloud_cloudauth-intl20220809-1.0.9/alibabacloud_cloudauth_intl20220809.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-05-05 07:43:50.000000 alibabacloud_cloudauth-intl20220809-1.0.9/alibabacloud_cloudauth_intl20220809.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      508 2023-05-05 07:43:50.000000 alibabacloud_cloudauth-intl20220809-1.0.9/alibabacloud_cloudauth_intl20220809.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 07:43:50.000000 alibabacloud_cloudauth-intl20220809-1.0.9/alibabacloud_cloudauth_intl20220809.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-05 07:43:50.000000 alibabacloud_cloudauth-intl20220809-1.0.9/alibabacloud_cloudauth_intl20220809.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-05 07:43:50.000000 alibabacloud_cloudauth-intl20220809-1.0.9/alibabacloud_cloudauth_intl20220809.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-05 07:43:51.000000 alibabacloud_cloudauth-intl20220809-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2667 2023-05-05 07:43:50.000000 alibabacloud_cloudauth-intl20220809-1.0.9/setup.py
```

### Comparing `alibabacloud_cloudauth-intl20220809-1.0.8/LICENSE` & `alibabacloud_cloudauth-intl20220809-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth-intl20220809-1.0.8/PKG-INFO` & `alibabacloud_cloudauth-intl20220809-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloudauth-intl20220809
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud Cloudauth-intl (20220809) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth-intl20220809-1.0.8/README-CN.md` & `alibabacloud_cloudauth-intl20220809-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth-intl20220809-1.0.8/README.md` & `alibabacloud_cloudauth-intl20220809-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809.egg-info/PKG-INFO` & `alibabacloud_cloudauth-intl20220809-1.0.9/alibabacloud_cloudauth_intl20220809.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloudauth-intl20220809
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud Cloudauth-intl (20220809) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth-intl20220809-1.0.8/setup.py` & `alibabacloud_cloudauth-intl20220809-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloudauth-intl20220809.
 
-Created on 19/04/2023
+Created on 05/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloudauth_intl20220809"
 NAME = "alibabacloud_cloudauth-intl20220809" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Cloudauth-intl (20220809) SDK Library for Python"
```

