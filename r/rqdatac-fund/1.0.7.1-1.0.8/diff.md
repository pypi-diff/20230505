# Comparing `tmp/rqdatac_fund-1.0.7.1.tar.gz` & `tmp/rqdatac_fund-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rqdatac_fund-1.0.7.1.tar", last modified: Mon Jul 27 10:18:22 2020, max compression
+gzip compressed data, was "dist\rqdatac_fund-1.0.8.tar", last modified: Wed Jul 29 10:41:46 2020, max compression
```

## Comparing `rqdatac_fund-1.0.7.1.tar` & `rqdatac_fund-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2020-07-27 10:18:22.000000 rqdatac_fund-1.0.7.1/
--rw-rw-rw-   0        0        0        0 2020-06-10 11:56:32.000000 rqdatac_fund-1.0.7.1/HISTORY.md
--rw-rw-rw-   0        0        0      180 2020-06-10 11:56:32.000000 rqdatac_fund-1.0.7.1/MANIFEST.in
--rw-rw-rw-   0        0        0      876 2020-07-27 10:18:22.000000 rqdatac_fund-1.0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0       44 2020-06-10 11:56:32.000000 rqdatac_fund-1.0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2020-07-27 10:18:22.000000 rqdatac_fund-1.0.7.1/rqdatac_fund/
--rw-rw-rw-   0        0        0      181 2020-06-11 08:41:20.000000 rqdatac_fund-1.0.7.1/rqdatac_fund/__init__.py
--rw-rw-rw-   0        0        0      520 2020-07-27 10:18:22.000000 rqdatac_fund-1.0.7.1/rqdatac_fund/_version.py
--rw-rw-rw-   0        0        0    44848 2020-07-27 03:56:03.000000 rqdatac_fund-1.0.7.1/rqdatac_fund/api.py
-drwxrwxrwx   0        0        0        0 2020-07-27 10:18:22.000000 rqdatac_fund-1.0.7.1/rqdatac_fund.egg-info/
--rw-rw-rw-   0        0        0      876 2020-07-27 10:18:22.000000 rqdatac_fund-1.0.7.1/rqdatac_fund.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2020-07-27 10:18:22.000000 rqdatac_fund-1.0.7.1/rqdatac_fund.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-07-27 10:18:22.000000 rqdatac_fund-1.0.7.1/rqdatac_fund.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2020-07-27 10:18:22.000000 rqdatac_fund-1.0.7.1/rqdatac_fund.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2020-06-11 02:29:23.000000 rqdatac_fund-1.0.7.1/rqdatac_fund.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       37 2020-07-27 10:18:22.000000 rqdatac_fund-1.0.7.1/rqdatac_fund.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2020-07-27 10:18:22.000000 rqdatac_fund-1.0.7.1/rqdatac_fund.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      236 2020-07-27 10:18:22.000000 rqdatac_fund-1.0.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1512 2020-07-24 05:59:13.000000 rqdatac_fund-1.0.7.1/setup.py
--rw-rw-rw-   0        0        0    69945 2020-06-10 11:56:32.000000 rqdatac_fund-1.0.7.1/versioneer.py
+drwxrwxrwx   0        0        0        0 2020-07-29 10:41:46.000000 rqdatac_fund-1.0.8/
+-rw-rw-rw-   0        0        0        0 2020-06-10 11:56:32.000000 rqdatac_fund-1.0.8/HISTORY.md
+-rw-rw-rw-   0        0        0      180 2020-06-10 11:56:32.000000 rqdatac_fund-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      874 2020-07-29 10:41:46.000000 rqdatac_fund-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2020-06-10 11:56:32.000000 rqdatac_fund-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2020-07-29 10:41:46.000000 rqdatac_fund-1.0.8/rqdatac_fund/
+-rw-rw-rw-   0        0        0      181 2020-06-11 08:41:20.000000 rqdatac_fund-1.0.8/rqdatac_fund/__init__.py
+-rw-rw-rw-   0        0        0      518 2020-07-29 10:41:46.000000 rqdatac_fund-1.0.8/rqdatac_fund/_version.py
+-rw-rw-rw-   0        0        0    45524 2020-07-28 09:29:51.000000 rqdatac_fund-1.0.8/rqdatac_fund/api.py
+drwxrwxrwx   0        0        0        0 2020-07-29 10:41:46.000000 rqdatac_fund-1.0.8/rqdatac_fund.egg-info/
+-rw-rw-rw-   0        0        0      874 2020-07-29 10:41:46.000000 rqdatac_fund-1.0.8/rqdatac_fund.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2020-07-29 10:41:46.000000 rqdatac_fund-1.0.8/rqdatac_fund.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-07-29 10:41:46.000000 rqdatac_fund-1.0.8/rqdatac_fund.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2020-07-29 10:41:46.000000 rqdatac_fund-1.0.8/rqdatac_fund.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2020-06-11 02:29:23.000000 rqdatac_fund-1.0.8/rqdatac_fund.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       37 2020-07-29 10:41:46.000000 rqdatac_fund-1.0.8/rqdatac_fund.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2020-07-29 10:41:46.000000 rqdatac_fund-1.0.8/rqdatac_fund.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      236 2020-07-29 10:41:46.000000 rqdatac_fund-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1512 2020-07-28 05:58:12.000000 rqdatac_fund-1.0.8/setup.py
+-rw-rw-rw-   0        0        0    69945 2020-06-10 11:56:32.000000 rqdatac_fund-1.0.8/versioneer.py
```

### Comparing `rqdatac_fund-1.0.7.1/PKG-INFO` & `rqdatac_fund-1.0.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: rqdatac_fund
-Version: 1.0.7.1
+Version: 1.0.8
 Summary: rqdatac fund extension
 Home-page: https://www.ricequant.com/
 Author: Ricequant
 Author-email: public@ricequant.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: rqdatac_fund
```

### Comparing `rqdatac_fund-1.0.7.1/rqdatac_fund/_version.py` & `rqdatac_fund-1.0.8/rqdatac_fund/_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2020-07-24T15:17:19+0800",
+ "date": "2020-07-28T17:39:06+0800",
  "dirty": false,
  "error": null,
- "full-revisionid": "bae7d88d00281ccb9808544f6b4fcb3853bc36a5",
- "version": "1.0.7.1"
+ "full-revisionid": "0fe914f7dc2cb8636fce6eef87a6400352d10159",
+ "version": "1.0.8"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

### Comparing `rqdatac_fund-1.0.7.1/rqdatac_fund/api.py` & `rqdatac_fund-1.0.8/rqdatac_fund/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 import datetime
 import warnings
+from collections import defaultdict
 
 import numpy as np
 import pandas as pd
 from dateutil.relativedelta import relativedelta
 from rqdatac.client import get_client
 from rqdatac.decorators import export_as_api, ttl_cache
 from rqdatac.services.basic import Instrument
@@ -15,14 +16,15 @@
     ensure_date_int,
     ensure_list_of_string,
     ensure_string_in,
     check_items_in_container,
     ensure_trading_date,
     ensure_date_range,
     raise_for_no_panel,
+    check_type
 )
 
 
 def _get_instrument(order_book_id, market="cn"):
     d = _all_instruments_dict(market)
     return d.get(order_book_id)
 
@@ -209,42 +211,14 @@
         else:
             field = result.columns[0]
             result = result.unstack(0)[field]
 
         return result
 
 
-CATEGORY_MAP = {
-    1: 'AShare',
-    3: 'Warrant',
-    4: 'Fund',
-    6: 'GovernmentBond',
-    7: 'FinancialBond',
-    8: 'Fund',
-    9: 'ConvertibleBond',
-    11: 'CorporateBond',
-    13: 'Fund',
-    14: 'BankNotes',
-    17: 'ABS',
-    18: 'ABS1',
-    20: 'Warrant',
-    21: 'Warrant',
-    22: 'IndexFutures',
-    28: 'LocalGovernmentBond',
-    29: 'ExchangeableBond',
-    33: 'CertificateOfDeposit',
-    51: 'HShare',
-    53: 'HShare',
-    60: 'Fund',
-    65: 'DebtSecu',
-    76: 'GovernmentBondFutures',
-    77: 'CommodityFutures',
-}
-
-
 @export_as_api(namespace="fund")
 def get_holdings(order_book_ids, date=None, market="cn", **kwargs):
     """获取距离指定日期最近发布的基金持仓信息
 
     :param order_book_ids: 基金代码，str 或 list of str
     :param date: 日期，为空则返回所有持仓 (Default value = None)
     :param market:  (Default value = "cn")
@@ -262,22 +236,21 @@
         elif "start_date" in kwargs or "end_date" in kwargs:
             raise ValueError('please ensure start_date and end_date exist')
         else:
             start_date = end_date = None
     if kwargs:
         raise ValueError('unknown kwargs: {}'.format(kwargs))
 
-    df = get_client().execute("fund.get_holdings_v3", order_book_ids, date, start_date, end_date, market=market)
+    df = get_client().execute("fund.get_holdings_v4", order_book_ids, date, start_date, end_date, market=market)
     if not df:
         return
 
     df = pd.DataFrame(data=df)
     fields = ["order_book_id", "type", "weight", "shares", "market_value", "symbol"]
     if "category" in df.columns:
-        df.category = df.category.map(CATEGORY_MAP)
         fields += ["category"]
     if "region" in df.columns:
         fields += ["region"]
 
     df.sort_values(["fund_id", "date", "type", "order_book_id"], inplace=True)
     df.set_index(["fund_id", "date"], inplace=True)
     return df[fields]
@@ -991,69 +964,57 @@
         ]
         df = pd.DataFrame.from_records(result, index=['order_book_id', 'category_type'], columns=c)
     else:
         df = pd.DataFrame.from_records(result, index=['order_book_id', 'category_type'])
     return df
 
 
-GET_CATEGORY_TYPES = {
-    'large', 'mid_cap', 'small',
-    'growth', 'blend', 'value',
-    'aggressive', 'active', 'flexible', 'balanced', 'moderate',
-    'interest_rate_bond', 'credit_bond', 'convertible_bond',
-    '1_year', '1_to_3_years', '3_to_5_years', '5_years',
-    '1013001', '1013002', '1013003',
-    '1014001', '1014002', '1014003',
-    '1015001', '1015002', '1015003', '1015004', '1015005',
-    '1110001', '1110002', '1110003',
-    '1111001', '1111002', '1111003', '1111004'
-}
-GET_CATEGORY_CODE2NAME_MAP = {
-    '1013001': 'large',
-    '1013002': 'mid_cap',
-    '1013003': 'small',
-    '1014001': 'growth',
-    '1014002': 'blend',
-    '1014003': 'value',
-    '1015001': 'aggressive',
-    '1015002': 'active',
-    '1015003': 'flexible',
-    '1015004': 'balanced',
-    '1015005': 'moderate',
-    '1110001': 'interest_rate_bond',
-    '1110002': 'credit_bond',
-    '1110003': 'convertible_bond',
-    '1111001': '1_year',
-    '1111002': '1_to_3_years',
-    '1111003': '3_to_5_years',
-    '1111004': '5_years'
-}
-
-
 @export_as_api(namespace='fund')
-def get_category(category, date=None, source='gildata', market="cn"):
+def get_category(category, date=None, source='gildata', market='cn'):
     """获取指定分类下所属基金列表
 
-    :param category: 风格名称或代码，可为字符串或字符串列表，如果为列表，则表示选取同时具有这些风格的基金，可选值：'large', 'mid_cap', 'small', 'growth', 'blend', 'value', 'aggressive', 'active', 'flexible', 'balanced', 'moderate', 'interest_rate_bond', 'credit_bond', 'convertible_bond', '1_year', '1_to_3_years', '3_to_5_years', '5_years' 或 '1013001', '1013002', '1013003', '1014001', '1014002', '1014003', '1015001', '1015002', '1015003', '1015004', '1015005', '1110001', '1110002', '1110003', '1111001', '1111002', '1111003', '1111004'
+    :param category: 风格类型映射, 如{"concept": ["食品饮料", "国防军工"], "investment_style": "沪港深混合型"}
     :param date: 如 '2015-01-07' 或 '20150107' (Default value = None)
     :param source: 分类来源。gildata: 聚源
     :param market:  (Default value = "cn")
     :returns: DataFrame
     """
+    category_keys = {
+        'value', 'size', 'operating_style', 'duration', 'bond_type', 'fund_type',
+        'industry_citics', 'concept', 'investment_style', 'universe', 'structured_fund'
+    }
 
     if date:
         date = ensure_date_int(date)
 
-    category = ensure_list_of_string(category)
-    check_items_in_container(category, GET_CATEGORY_TYPES, 'category_type')
-    category = list(set(GET_CATEGORY_CODE2NAME_MAP.get(x, x) for x in category))
-
+    check_type(category, dict, "category")
     source = ensure_string_in(source, {'gildata'}, 'source')
 
-    return get_client().execute('fund.get_category', category, date, source, market=market)
+    check_items_in_container(category, category_keys, 'category')
+    for k in category:
+        category[k] = ensure_list_of_string(category[k])
+
+    category_types_map = defaultdict(list)
+
+    category_type_copy = list(category.keys())
+    if "fund_type" in category_type_copy:
+        fund_type_df = get_category_mapping(category_type="fund_type")
+        category_types_map["fund_type"].extend(fund_type_df.values.flatten().tolist())
+        category_type_copy.remove("fund_type")
+
+    if category_type_copy:
+        df = get_category_mapping(category_type=category_type_copy)
+        unique_index = df.index.unique()
+        for idx in unique_index:
+            category_types_map[idx].extend([_ for _ in df.loc[idx].values.flatten() if _ is not None])
+
+    for c in category:
+        if not set(category[c]).issubset(set(category_types_map[c])):
+            raise ValueError("Unexpected category.")
+    return get_client().execute('fund.get_category_v2', category, date, source, market=market)
 
 
 @export_as_api(namespace='fund')
 def get_category_mapping(source='gildata', category_type=None, market="cn"):
     """获取风格分类列表概览
 
     :param source: 分类来源。gildata: 聚源
@@ -1275,7 +1236,57 @@
         lambda g: g if 1 < len(g) else pd.DataFrame())
     df.dropna(inplace=True)
     if 0 == len(df):
         return
     df["transition_time"] = df["transition_time"].astype(int)
     df.set_index(["order_book_id", "transition_time"], inplace=True)
     return df
+
+
+TRANSACTION_STATUS_FIELDS = [
+    "subscribe_status",
+    "redeem_status",
+    "subscribe_upper_limit",
+    "subscribe_lower_limit",
+    "redeem_lower_limit",
+]
+
+
+@export_as_api(namespace="fund")
+def get_transaction_status(order_book_ids, start_date=None, end_date=None, fields=None, investor="institution",
+                         market="cn"):
+    """获取基金净值数据
+
+    :param order_book_ids: 基金代码，str 或 list of str
+    :param start_date: 开始日期 (Default value = None)
+    :param end_date: 结束日期 (Default value = None)
+    :param fields: str or list of str，例如：'subscribe_status', 'redeem_status',
+                    'subscribe_upper_limit', 'subscribe_lower_limit', 'redeem_lower_limit' (Default value = None)
+    :param investor: 投资者身份(Default value = institution) institution/retail
+    :param market:  (Default value = "cn")
+    :returns: DataFrame
+
+    """
+    order_book_ids = ensure_list_of_string(order_book_ids)
+
+    if start_date:
+        start_date = ensure_date_int(start_date)
+    if end_date:
+        end_date = ensure_date_int(end_date)
+
+    if fields is not None:
+        fields = ensure_list_of_string(fields)
+        check_items_in_container(fields, TRANSACTION_STATUS_FIELDS, 'invalid field')
+    else:
+        fields = TRANSACTION_STATUS_FIELDS
+
+    result = get_client().execute(
+        "fund.get_transaction_status", order_book_ids, start_date, end_date, fields, investor=investor, market=market
+    )
+    if not result:
+        return
+    result = pd.DataFrame(result)
+    result.set_index(["order_book_id", "datetime"], inplace=True)
+    result.sort_index(inplace=True)
+    result = result[fields]
+    result = result.where(result.notnull(), None)
+    return result
```

### Comparing `rqdatac_fund-1.0.7.1/rqdatac_fund.egg-info/PKG-INFO` & `rqdatac_fund-1.0.8/rqdatac_fund.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: rqdatac-fund
-Version: 1.0.7.1
+Version: 1.0.8
 Summary: rqdatac fund extension
 Home-page: https://www.ricequant.com/
 Author: Ricequant
 Author-email: public@ricequant.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: rqdatac_fund
```

### Comparing `rqdatac_fund-1.0.7.1/setup.py` & `rqdatac_fund-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `rqdatac_fund-1.0.7.1/versioneer.py` & `rqdatac_fund-1.0.8/versioneer.py`

 * *Files identical despite different names*

