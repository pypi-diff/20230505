# Comparing `tmp/alibabacloud_imagesearch20210501-1.2.2.tar.gz` & `tmp/alibabacloud_imagesearch20210501-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_imagesearch20210501-1.2.2.tar", last modified: Tue Jan 10 09:17:46 2023, max compression
+gzip compressed data, was "dist/alibabacloud_imagesearch20210501-1.2.3.tar", last modified: Fri May  5 06:37:52 2023, max compression
```

## Comparing `alibabacloud_imagesearch20210501-1.2.2.tar` & `alibabacloud_imagesearch20210501-1.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 09:17:46.000000 alibabacloud_imagesearch20210501-1.2.2/
--rw-r--r--   0 root         (0) root         (0)      371 2023-01-10 09:17:45.000000 alibabacloud_imagesearch20210501-1.2.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-01-10 09:17:45.000000 alibabacloud_imagesearch20210501-1.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-01-10 09:17:45.000000 alibabacloud_imagesearch20210501-1.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2377 2023-01-10 09:17:46.000000 alibabacloud_imagesearch20210501-1.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1046 2023-01-10 09:17:45.000000 alibabacloud_imagesearch20210501-1.2.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2023-01-10 09:17:45.000000 alibabacloud_imagesearch20210501-1.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 09:17:46.000000 alibabacloud_imagesearch20210501-1.2.2/alibabacloud_imagesearch20210501/
--rw-r--r--   0 root         (0) root         (0)       21 2023-01-10 09:17:45.000000 alibabacloud_imagesearch20210501-1.2.2/alibabacloud_imagesearch20210501/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21077 2023-01-10 09:17:45.000000 alibabacloud_imagesearch20210501-1.2.2/alibabacloud_imagesearch20210501/client.py
--rw-r--r--   0 root         (0) root         (0)    63543 2023-01-10 09:17:45.000000 alibabacloud_imagesearch20210501-1.2.2/alibabacloud_imagesearch20210501/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 09:17:46.000000 alibabacloud_imagesearch20210501-1.2.2/alibabacloud_imagesearch20210501.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2377 2023-01-10 09:17:45.000000 alibabacloud_imagesearch20210501-1.2.2/alibabacloud_imagesearch20210501.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2023-01-10 09:17:46.000000 alibabacloud_imagesearch20210501-1.2.2/alibabacloud_imagesearch20210501.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-10 09:17:45.000000 alibabacloud_imagesearch20210501-1.2.2/alibabacloud_imagesearch20210501.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      315 2023-01-10 09:17:45.000000 alibabacloud_imagesearch20210501-1.2.2/alibabacloud_imagesearch20210501.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-01-10 09:17:45.000000 alibabacloud_imagesearch20210501-1.2.2/alibabacloud_imagesearch20210501.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-01-10 09:17:46.000000 alibabacloud_imagesearch20210501-1.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2842 2023-01-10 09:17:45.000000 alibabacloud_imagesearch20210501-1.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:37:52.000000 alibabacloud_imagesearch20210501-1.2.3/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-05 06:37:52.000000 alibabacloud_imagesearch20210501-1.2.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-05 06:37:52.000000 alibabacloud_imagesearch20210501-1.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-05 06:37:52.000000 alibabacloud_imagesearch20210501-1.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2377 2023-05-05 06:37:52.000000 alibabacloud_imagesearch20210501-1.2.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-05-05 06:37:52.000000 alibabacloud_imagesearch20210501-1.2.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-05-05 06:37:52.000000 alibabacloud_imagesearch20210501-1.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:37:52.000000 alibabacloud_imagesearch20210501-1.2.3/alibabacloud_imagesearch20210501/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-05 06:37:52.000000 alibabacloud_imagesearch20210501-1.2.3/alibabacloud_imagesearch20210501/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21077 2023-05-05 06:37:52.000000 alibabacloud_imagesearch20210501-1.2.3/alibabacloud_imagesearch20210501/client.py
+-rw-r--r--   0 root         (0) root         (0)    63818 2023-05-05 06:37:52.000000 alibabacloud_imagesearch20210501-1.2.3/alibabacloud_imagesearch20210501/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:37:52.000000 alibabacloud_imagesearch20210501-1.2.3/alibabacloud_imagesearch20210501.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2377 2023-05-05 06:37:52.000000 alibabacloud_imagesearch20210501-1.2.3/alibabacloud_imagesearch20210501.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2023-05-05 06:37:52.000000 alibabacloud_imagesearch20210501-1.2.3/alibabacloud_imagesearch20210501.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 06:37:52.000000 alibabacloud_imagesearch20210501-1.2.3/alibabacloud_imagesearch20210501.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      315 2023-05-05 06:37:52.000000 alibabacloud_imagesearch20210501-1.2.3/alibabacloud_imagesearch20210501.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-05-05 06:37:52.000000 alibabacloud_imagesearch20210501-1.2.3/alibabacloud_imagesearch20210501.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-05 06:37:52.000000 alibabacloud_imagesearch20210501-1.2.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-05-05 06:37:52.000000 alibabacloud_imagesearch20210501-1.2.3/setup.py
```

### Comparing `alibabacloud_imagesearch20210501-1.2.2/LICENSE` & `alibabacloud_imagesearch20210501-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_imagesearch20210501-1.2.2/PKG-INFO` & `alibabacloud_imagesearch20210501-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_imagesearch20210501
-Version: 1.2.2
+Version: 1.2.3
 Summary: Alibaba Cloud image search (20210501) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_imagesearch20210501-1.2.2/README-CN.md` & `alibabacloud_imagesearch20210501-1.2.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_imagesearch20210501-1.2.2/README.md` & `alibabacloud_imagesearch20210501-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_imagesearch20210501-1.2.2/alibabacloud_imagesearch20210501/client.py` & `alibabacloud_imagesearch20210501-1.2.3/alibabacloud_imagesearch20210501/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_imagesearch20210501-1.2.2/alibabacloud_imagesearch20210501/models.py` & `alibabacloud_imagesearch20210501-1.2.3/alibabacloud_imagesearch20210501/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
         coupon_remain_count: int = None,
         coupon_share_url: str = None,
         coupon_start_fee: str = None,
         coupon_start_time: str = None,
         coupon_total_count: str = None,
         deeplink_coupon_share_url: str = None,
         deeplink_url: str = None,
+        input_item_id: str = None,
         item_id: str = None,
         level_one_category_name: str = None,
         max_commission: GetProductInfoByIdsResponseBodyDataAuctionsResultMaxCommission = None,
         nick: str = None,
         pic_url: str = None,
         price_after_coupon: str = None,
         provcity: str = None,
@@ -123,14 +124,15 @@
         self.coupon_remain_count = coupon_remain_count
         self.coupon_share_url = coupon_share_url
         self.coupon_start_fee = coupon_start_fee
         self.coupon_start_time = coupon_start_time
         self.coupon_total_count = coupon_total_count
         self.deeplink_coupon_share_url = deeplink_coupon_share_url
         self.deeplink_url = deeplink_url
+        self.input_item_id = input_item_id
         self.item_id = item_id
         self.level_one_category_name = level_one_category_name
         self.max_commission = max_commission
         self.nick = nick
         self.pic_url = pic_url
         self.price_after_coupon = price_after_coupon
         self.provcity = provcity
@@ -175,14 +177,16 @@
             result['CouponStartTime'] = self.coupon_start_time
         if self.coupon_total_count is not None:
             result['CouponTotalCount'] = self.coupon_total_count
         if self.deeplink_coupon_share_url is not None:
             result['DeeplinkCouponShareUrl'] = self.deeplink_coupon_share_url
         if self.deeplink_url is not None:
             result['DeeplinkUrl'] = self.deeplink_url
+        if self.input_item_id is not None:
+            result['InputItemId'] = self.input_item_id
         if self.item_id is not None:
             result['ItemId'] = self.item_id
         if self.level_one_category_name is not None:
             result['LevelOneCategoryName'] = self.level_one_category_name
         if self.max_commission is not None:
             result['MaxCommission'] = self.max_commission.to_map()
         if self.nick is not None:
@@ -237,14 +241,16 @@
             self.coupon_start_time = m.get('CouponStartTime')
         if m.get('CouponTotalCount') is not None:
             self.coupon_total_count = m.get('CouponTotalCount')
         if m.get('DeeplinkCouponShareUrl') is not None:
             self.deeplink_coupon_share_url = m.get('DeeplinkCouponShareUrl')
         if m.get('DeeplinkUrl') is not None:
             self.deeplink_url = m.get('DeeplinkUrl')
+        if m.get('InputItemId') is not None:
+            self.input_item_id = m.get('InputItemId')
         if m.get('ItemId') is not None:
             self.item_id = m.get('ItemId')
         if m.get('LevelOneCategoryName') is not None:
             self.level_one_category_name = m.get('LevelOneCategoryName')
         if m.get('MaxCommission') is not None:
             temp_model = GetProductInfoByIdsResponseBodyDataAuctionsResultMaxCommission()
             self.max_commission = temp_model.from_map(m['MaxCommission'])
```

### Comparing `alibabacloud_imagesearch20210501-1.2.2/alibabacloud_imagesearch20210501.egg-info/PKG-INFO` & `alibabacloud_imagesearch20210501-1.2.3/alibabacloud_imagesearch20210501.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-imagesearch20210501
-Version: 1.2.2
+Version: 1.2.3
 Summary: Alibaba Cloud image search (20210501) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_imagesearch20210501-1.2.2/setup.py` & `alibabacloud_imagesearch20210501-1.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_imagesearch20210501.
 
-Created on 10/01/2023
+Created on 05/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_imagesearch20210501"
 NAME = "alibabacloud_imagesearch20210501" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud image search (20210501) SDK Library for Python"
@@ -39,15 +39,15 @@
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_oss_sdk>=0.1.0, <1.0.0",
     "alibabacloud_openplatform20191219>=2.0.0, <3.0.0",
     "alibabacloud_oss_util>=0.0.5, <1.0.0",
     "alibabacloud_tea_fileform>=0.0.3, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.0, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

