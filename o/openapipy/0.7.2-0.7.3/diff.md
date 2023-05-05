# Comparing `tmp/openapipy-0.7.2.tar.gz` & `tmp/openapipy-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapipy-0.7.2.tar", last modified: Tue May  2 01:21:16 2023, max compression
+gzip compressed data, was "openapipy-0.7.3.tar", last modified: Fri May  5 10:02:00 2023, max compression
```

## Comparing `openapipy-0.7.2.tar` & `openapipy-0.7.3.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:21:16.627048 openapipy-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-02 01:20:58.000000 openapipy-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-02 01:21:16.627048 openapipy-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-02 01:20:58.000000 openapipy-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:21:16.623048 openapipy-0.7.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:21:16.623048 openapipy-0.7.2/examples/alipay/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/alipay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/alipay/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:21:16.623048 openapipy-0.7.2/examples/aliyun/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/aliyun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/aliyun/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:21:16.623048 openapipy-0.7.2/examples/doudian/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/doudian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/doudian/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:21:16.623048 openapipy-0.7.2/examples/feishu/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/feishu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/feishu/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/feishu/sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:21:16.623048 openapipy-0.7.2/examples/lenovo/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/lenovo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/lenovo/pay.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/lenovo/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/lenovo/sign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:21:16.623048 openapipy-0.7.2/examples/sms/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/sms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/sms/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:21:16.623048 openapipy-0.7.2/examples/tanmarket/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/tanmarket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/tanmarket/bulk_gonghai.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/tanmarket/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/tanmarket/field_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/tanmarket/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/tanmarket/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:21:16.627048 openapipy-0.7.2/examples/wechat/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/wechat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/wechat/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/wechat/open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/wechat/pay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:21:16.627048 openapipy-0.7.2/examples/xiaoetong/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/xiaoetong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/xiaoetong/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:21:16.627048 openapipy-0.7.2/examples/yizhi/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/yizhi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/yizhi/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/yizhi/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:21:16.627048 openapipy-0.7.2/examples/yunduo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/yunduo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-02 01:20:58.000000 openapipy-0.7.2/examples/yunduo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:21:16.627048 openapipy-0.7.2/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:21:16.627048 openapipy-0.7.2/openapi/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/alipay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/aliyun.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:21:16.627048 openapipy-0.7.2/openapi/providers/crm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/crm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/crm/tanmarket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/crm/yunduo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/doudian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:21:16.627048 openapipy-0.7.2/openapi/providers/feishu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/feishu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/feishu/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/feishu/open.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/lenovo.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/polyv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:21:16.627048 openapipy-0.7.2/openapi/providers/sms/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/sms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/sms/submail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:21:16.627048 openapipy-0.7.2/openapi/providers/wechat/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/wechat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/wechat/open.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/wechat/pay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/xiaoetong.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/providers/yizhi.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-02 01:20:58.000000 openapipy-0.7.2/openapi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:21:16.627048 openapipy-0.7.2/openapipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-02 01:21:16.000000 openapipy-0.7.2/openapipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-02 01:21:16.000000 openapipy-0.7.2/openapipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 01:21:16.000000 openapipy-0.7.2/openapipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 01:21:16.000000 openapipy-0.7.2/openapipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 01:21:16.000000 openapipy-0.7.2/openapipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 01:21:16.000000 openapipy-0.7.2/openapipy.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 01:21:16.627048 openapipy-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-02 01:20:58.000000 openapipy-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:02:00.514701 openapipy-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 10:01:44.000000 openapipy-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-05 10:02:00.514701 openapipy-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-05 10:01:44.000000 openapipy-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:02:00.510701 openapipy-0.7.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:02:00.510701 openapipy-0.7.3/examples/alipay/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/alipay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/alipay/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:02:00.510701 openapipy-0.7.3/examples/aliyun/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/aliyun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/aliyun/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:02:00.510701 openapipy-0.7.3/examples/doudian/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/doudian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/doudian/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:02:00.510701 openapipy-0.7.3/examples/feishu/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/feishu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/feishu/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/feishu/sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:02:00.510701 openapipy-0.7.3/examples/lenovo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/lenovo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/lenovo/pay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/lenovo/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/lenovo/sign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:02:00.510701 openapipy-0.7.3/examples/sms/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/sms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/sms/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:02:00.510701 openapipy-0.7.3/examples/tanmarket/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/tanmarket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/tanmarket/bulk_gonghai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/tanmarket/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/tanmarket/field_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/tanmarket/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/tanmarket/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:02:00.510701 openapipy-0.7.3/examples/wechat/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/wechat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/wechat/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/wechat/open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/wechat/pay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:02:00.510701 openapipy-0.7.3/examples/xiaoetong/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/xiaoetong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/xiaoetong/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:02:00.510701 openapipy-0.7.3/examples/yizhi/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/yizhi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/yizhi/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/yizhi/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:02:00.514701 openapipy-0.7.3/examples/yunduo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/yunduo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-05 10:01:44.000000 openapipy-0.7.3/examples/yunduo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:02:00.514701 openapipy-0.7.3/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:02:00.514701 openapipy-0.7.3/openapi/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/alipay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/aliyun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:02:00.514701 openapipy-0.7.3/openapi/providers/crm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/crm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/crm/tanmarket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/crm/yunduo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/doudian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:02:00.514701 openapipy-0.7.3/openapi/providers/feishu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/feishu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/feishu/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/feishu/open.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/lenovo.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/polyv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:02:00.514701 openapipy-0.7.3/openapi/providers/sms/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/sms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/sms/submail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:02:00.514701 openapipy-0.7.3/openapi/providers/wechat/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/wechat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/wechat/open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/wechat/pay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/xiaoetong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/providers/yizhi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-05 10:01:44.000000 openapipy-0.7.3/openapi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:02:00.514701 openapipy-0.7.3/openapipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-05 10:02:00.000000 openapipy-0.7.3/openapipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-05 10:02:00.000000 openapipy-0.7.3/openapipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:02:00.000000 openapipy-0.7.3/openapipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 10:02:00.000000 openapipy-0.7.3/openapipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 10:02:00.000000 openapipy-0.7.3/openapipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:02:00.000000 openapipy-0.7.3/openapipy.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 10:02:00.514701 openapipy-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-05 10:01:44.000000 openapipy-0.7.3/setup.py
```

### Comparing `openapipy-0.7.2/LICENSE` & `openapipy-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/PKG-INFO` & `openapipy-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapipy
-Version: 0.7.2
+Version: 0.7.3
 Summary: openapi tools
 Home-page: https://github.com/luffy-genius/openapi
 Author: ZhiChaoLiu
 Author-email: liuzhichao9527@gmail.com
 License: MIT
 Keywords: openapi,openapi-python,python-openapi,openapipy,pyopenapi
 Description-Content-Type: text/markdown
```

### Comparing `openapipy-0.7.2/README.md` & `openapipy-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/examples/alipay/main.py` & `openapipy-0.7.3/examples/alipay/main.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/examples/aliyun/main.py` & `openapipy-0.7.3/examples/aliyun/main.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/examples/feishu/sheet.py` & `openapipy-0.7.3/examples/feishu/sheet.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/examples/lenovo/__init__.py` & `openapipy-0.7.3/examples/lenovo/__init__.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/examples/lenovo/pay.py` & `openapipy-0.7.3/examples/lenovo/pay.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/examples/lenovo/sign.py` & `openapipy-0.7.3/examples/lenovo/sign.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/examples/sms/main.py` & `openapipy-0.7.3/examples/sms/main.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/examples/tanmarket/bulk_gonghai.py` & `openapipy-0.7.3/examples/tanmarket/bulk_gonghai.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/examples/tanmarket/create.py` & `openapipy-0.7.3/examples/tanmarket/create.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/examples/tanmarket/field_map.py` & `openapipy-0.7.3/examples/tanmarket/field_map.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/examples/tanmarket/query.py` & `openapipy-0.7.3/examples/tanmarket/query.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/examples/tanmarket/update.py` & `openapipy-0.7.3/examples/tanmarket/update.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/examples/wechat/oauth.py` & `openapipy-0.7.3/examples/wechat/oauth.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/examples/wechat/pay.py` & `openapipy-0.7.3/examples/wechat/pay.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/examples/xiaoetong/main.py` & `openapipy-0.7.3/examples/xiaoetong/main.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/examples/yizhi/query.py` & `openapipy-0.7.3/examples/yizhi/query.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/examples/yunduo/main.py` & `openapipy-0.7.3/examples/yunduo/main.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/openapi/enums.py` & `openapipy-0.7.3/openapi/enums.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/openapi/providers/alipay.py` & `openapipy-0.7.3/openapi/providers/alipay.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/openapi/providers/aliyun.py` & `openapipy-0.7.3/openapi/providers/aliyun.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/openapi/providers/base.py` & `openapipy-0.7.3/openapi/providers/base.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/openapi/providers/crm/tanmarket.py` & `openapipy-0.7.3/openapi/providers/crm/tanmarket.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/openapi/providers/crm/yunduo.py` & `openapipy-0.7.3/openapi/providers/crm/yunduo.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/openapi/providers/doudian.py` & `openapipy-0.7.3/openapi/providers/doudian.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/openapi/providers/feishu/bot.py` & `openapipy-0.7.3/openapi/providers/feishu/bot.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/openapi/providers/feishu/open.py` & `openapipy-0.7.3/openapi/providers/feishu/open.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/openapi/providers/lenovo.py` & `openapipy-0.7.3/openapi/providers/lenovo.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/openapi/providers/sms/submail.py` & `openapipy-0.7.3/openapi/providers/sms/submail.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/openapi/providers/wechat/open.py` & `openapipy-0.7.3/openapi/providers/wechat/open.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,26 +27,26 @@
         super().__init__()
         self.app_id = app_id
         self.secret = secret
         self.codes = Code
 
     def request(
         self, method, endpoint, params=None, data=None,
-        token_request=False, is_oauth=True,
+        token_request=False, is_oauth=True, replace_url=True,
     ):
         if not token_request:
             if params is None:
                 params = {}
 
             if 'access_token' not in params and not is_oauth:
                 params['access_token'] = self.access_token
 
         # Support wechat oauth login
         api_base_url = self.API_BASE_URL
-        if not is_oauth:
+        if not is_oauth and replace_url:
             api_base_url = self.API_BASE_URL.replace('/cgi-bin', '')
 
         request_url = f'{api_base_url}{endpoint}'
         response = self._request(
             method, request_url,
             params=params, json=data
         )
```

### Comparing `openapipy-0.7.2/openapi/providers/wechat/pay.py` & `openapipy-0.7.3/openapi/providers/wechat/pay.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/openapi/providers/xiaoetong.py` & `openapipy-0.7.3/openapi/providers/xiaoetong.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/openapi/providers/yizhi.py` & `openapipy-0.7.3/openapi/providers/yizhi.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/openapi/utils.py` & `openapipy-0.7.3/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/openapipy.egg-info/PKG-INFO` & `openapipy-0.7.3/openapipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapipy
-Version: 0.7.2
+Version: 0.7.3
 Summary: openapi tools
 Home-page: https://github.com/luffy-genius/openapi
 Author: ZhiChaoLiu
 Author-email: liuzhichao9527@gmail.com
 License: MIT
 Keywords: openapi,openapi-python,python-openapi,openapipy,pyopenapi
 Description-Content-Type: text/markdown
```

### Comparing `openapipy-0.7.2/openapipy.egg-info/SOURCES.txt` & `openapipy-0.7.3/openapipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openapipy-0.7.2/setup.py` & `openapipy-0.7.3/setup.py`

 * *Files identical despite different names*

