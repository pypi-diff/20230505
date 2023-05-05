# Comparing `tmp/adata-0.0.6b0.tar.gz` & `tmp/adata-0.0.7b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adata-0.0.6b0.tar", last modified: Fri May  5 15:02:37 2023, max compression
+gzip compressed data, was "adata-0.0.7b0.tar", last modified: Fri May  5 15:09:54 2023, max compression
```

## Comparing `adata-0.0.6b0.tar` & `adata-0.0.7b0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 15:02:37.097794 adata-0.0.6b0/
--rw-rw-rw-   0        0        0      186 2023-04-06 11:14:06.000000 adata-0.0.6b0/HISTORY.md
--rw-rw-rw-   0        0        0    11558 2023-04-05 02:53:34.000000 adata-0.0.6b0/LICENSE
--rw-rw-rw-   0        0        0       27 2023-04-06 11:14:06.000000 adata-0.0.6b0/MANIFEST.in
--rw-rw-rw-   0        0        0     7151 2023-05-05 15:02:37.096794 adata-0.0.6b0/PKG-INFO
--rw-rw-rw-   0        0        0     6512 2023-04-25 16:01:44.000000 adata-0.0.6b0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 15:02:36.632200 adata-0.0.6b0/adata/
--rw-rw-rw-   0        0        0      545 2023-04-05 04:59:22.000000 adata-0.0.6b0/adata/__init__.py
--rw-rw-rw-   0        0        0      756 2023-05-05 15:02:16.000000 adata-0.0.6b0/adata/__version__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:02:36.652200 adata-0.0.6b0/adata/bond/
--rw-rw-rw-   0        0        0      122 2023-04-06 11:14:06.000000 adata-0.0.6b0/adata/bond/__init__.py
--rw-rw-rw-   0        0        0      203 2023-04-05 09:48:31.000000 adata-0.0.6b0/adata/bond/bond_market.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:02:36.654202 adata-0.0.6b0/adata/common/
--rw-rw-rw-   0        0        0      150 2023-04-05 09:48:31.000000 adata-0.0.6b0/adata/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:02:36.702203 adata-0.0.6b0/adata/common/headers/
--rw-rw-rw-   0        0        0      104 2023-04-05 09:48:30.000000 adata-0.0.6b0/adata/common/headers/__init__.py
--rw-rw-rw-   0        0        0     5772 2023-04-05 09:48:28.000000 adata-0.0.6b0/adata/common/headers/baidu_headers.py
--rw-rw-rw-   0        0        0      602 2023-04-18 15:14:02.000000 adata-0.0.6b0/adata/common/headers/sina_headers.py
--rw-rw-rw-   0        0        0     2999 2023-04-05 09:48:30.000000 adata-0.0.6b0/adata/common/headers/ths_headers.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:02:36.706201 adata-0.0.6b0/adata/common/js/
--rw-rw-rw-   0        0        0       99 2023-05-05 13:46:05.000000 adata-0.0.6b0/adata/common/js/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:02:37.014794 adata-0.0.6b0/adata/common/utils/
--rw-rw-rw-   0        0        0      205 2023-04-05 09:53:12.000000 adata-0.0.6b0/adata/common/utils/__init__.py
--rw-rw-rw-   0        0        0      753 2023-05-05 13:46:05.000000 adata-0.0.6b0/adata/common/utils/cookie.py
--rw-rw-rw-   0        0        0     3046 2023-04-05 09:48:27.000000 adata-0.0.6b0/adata/common/utils/snowflake.py
--rw-rw-rw-   0        0        0      979 2023-04-24 16:42:55.000000 adata-0.0.6b0/adata/common/utils/sunrequests.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:02:37.018826 adata-0.0.6b0/adata/etf/
--rw-rw-rw-   0        0        0      118 2023-04-06 11:14:06.000000 adata-0.0.6b0/adata/etf/__init__.py
--rw-rw-rw-   0        0        0      201 2023-04-05 09:48:28.000000 adata-0.0.6b0/adata/etf/etf_market.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:02:37.020829 adata-0.0.6b0/adata/message/
--rw-rw-rw-   0        0        0      103 2023-04-05 09:48:30.000000 adata-0.0.6b0/adata/message/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:02:37.022826 adata-0.0.6b0/adata/stock/
--rw-rw-rw-   0        0        0      333 2023-04-06 11:14:06.000000 adata-0.0.6b0/adata/stock/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:02:37.025825 adata-0.0.6b0/adata/stock/index/
--rw-rw-rw-   0        0        0      105 2023-04-06 11:14:06.000000 adata-0.0.6b0/adata/stock/index/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:02:37.035796 adata-0.0.6b0/adata/stock/info/
--rw-rw-rw-   0        0        0      380 2023-05-05 13:46:05.000000 adata-0.0.6b0/adata/stock/info/__init__.py
--rw-rw-rw-   0        0        0     2550 2023-04-25 15:29:33.000000 adata-0.0.6b0/adata/stock/info/stock_code.py
--rw-rw-rw-   0        0        0     6722 2023-05-05 14:49:14.000000 adata-0.0.6b0/adata/stock/info/stock_concept.py
--rw-rw-rw-   0        0        0     2027 2023-05-05 14:11:27.000000 adata-0.0.6b0/adata/stock/info/trade_calendar.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:02:37.091794 adata-0.0.6b0/adata/stock/market/
--rw-rw-rw-   0        0        0      408 2023-04-13 14:47:15.000000 adata-0.0.6b0/adata/stock/market/__init__.py
--rw-rw-rw-   0        0        0     2941 2023-04-20 13:03:47.000000 adata-0.0.6b0/adata/stock/market/stock_dividend.py
--rw-rw-rw-   0        0        0    10485 2023-04-25 15:43:53.000000 adata-0.0.6b0/adata/stock/market/stock_market.py
--rw-rw-rw-   0        0        0     8363 2023-04-25 15:49:26.000000 adata-0.0.6b0/adata/stock/market/stock_market_concept.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:02:37.093794 adata-0.0.6b0/adata/stock/sentiment/
--rw-rw-rw-   0        0        0      115 2023-04-06 11:14:06.000000 adata-0.0.6b0/adata/stock/sentiment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:02:36.646200 adata-0.0.6b0/adata.egg-info/
--rw-rw-rw-   0        0        0     7151 2023-05-05 15:02:36.000000 adata-0.0.6b0/adata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1056 2023-05-05 15:02:36.000000 adata-0.0.6b0/adata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 15:02:36.000000 adata-0.0.6b0/adata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-05-05 15:02:36.000000 adata-0.0.6b0/adata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-05 15:02:36.000000 adata-0.0.6b0/adata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-05-05 13:46:05.000000 adata-0.0.6b0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 15:02:37.097794 adata-0.0.6b0/setup.cfg
--rw-rw-rw-   0        0        0     1790 2023-04-18 15:37:51.000000 adata-0.0.6b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:09:54.407912 adata-0.0.7b0/
+-rw-rw-rw-   0        0        0      186 2023-04-06 11:14:06.000000 adata-0.0.7b0/HISTORY.md
+-rw-rw-rw-   0        0        0    11558 2023-04-05 02:53:34.000000 adata-0.0.7b0/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-04-06 11:14:06.000000 adata-0.0.7b0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7151 2023-05-05 15:09:54.406911 adata-0.0.7b0/PKG-INFO
+-rw-rw-rw-   0        0        0     6512 2023-04-25 16:01:44.000000 adata-0.0.7b0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 15:09:54.307912 adata-0.0.7b0/adata/
+-rw-rw-rw-   0        0        0      545 2023-04-05 04:59:22.000000 adata-0.0.7b0/adata/__init__.py
+-rw-rw-rw-   0        0        0      756 2023-05-05 15:09:50.000000 adata-0.0.7b0/adata/__version__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:09:54.325913 adata-0.0.7b0/adata/bond/
+-rw-rw-rw-   0        0        0      122 2023-04-06 11:14:06.000000 adata-0.0.7b0/adata/bond/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-04-05 09:48:31.000000 adata-0.0.7b0/adata/bond/bond_market.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:09:54.327913 adata-0.0.7b0/adata/common/
+-rw-rw-rw-   0        0        0      150 2023-04-05 09:48:31.000000 adata-0.0.7b0/adata/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:09:54.345018 adata-0.0.7b0/adata/common/headers/
+-rw-rw-rw-   0        0        0      104 2023-04-05 09:48:30.000000 adata-0.0.7b0/adata/common/headers/__init__.py
+-rw-rw-rw-   0        0        0     5772 2023-04-05 09:48:28.000000 adata-0.0.7b0/adata/common/headers/baidu_headers.py
+-rw-rw-rw-   0        0        0      602 2023-04-18 15:14:02.000000 adata-0.0.7b0/adata/common/headers/sina_headers.py
+-rw-rw-rw-   0        0        0     2999 2023-04-05 09:48:30.000000 adata-0.0.7b0/adata/common/headers/ths_headers.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:09:54.347915 adata-0.0.7b0/adata/common/js/
+-rw-rw-rw-   0        0        0       99 2023-05-05 13:46:05.000000 adata-0.0.7b0/adata/common/js/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:09:54.357912 adata-0.0.7b0/adata/common/utils/
+-rw-rw-rw-   0        0        0      205 2023-04-05 09:53:12.000000 adata-0.0.7b0/adata/common/utils/__init__.py
+-rw-rw-rw-   0        0        0      753 2023-05-05 13:46:05.000000 adata-0.0.7b0/adata/common/utils/cookie.py
+-rw-rw-rw-   0        0        0     3046 2023-04-05 09:48:27.000000 adata-0.0.7b0/adata/common/utils/snowflake.py
+-rw-rw-rw-   0        0        0      979 2023-04-24 16:42:55.000000 adata-0.0.7b0/adata/common/utils/sunrequests.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:09:54.361912 adata-0.0.7b0/adata/etf/
+-rw-rw-rw-   0        0        0      118 2023-04-06 11:14:06.000000 adata-0.0.7b0/adata/etf/__init__.py
+-rw-rw-rw-   0        0        0      201 2023-04-05 09:48:28.000000 adata-0.0.7b0/adata/etf/etf_market.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:09:54.363911 adata-0.0.7b0/adata/message/
+-rw-rw-rw-   0        0        0      103 2023-04-05 09:48:30.000000 adata-0.0.7b0/adata/message/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:09:54.366913 adata-0.0.7b0/adata/stock/
+-rw-rw-rw-   0        0        0      333 2023-04-06 11:14:06.000000 adata-0.0.7b0/adata/stock/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:09:54.368942 adata-0.0.7b0/adata/stock/index/
+-rw-rw-rw-   0        0        0      105 2023-04-06 11:14:06.000000 adata-0.0.7b0/adata/stock/index/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:09:54.377944 adata-0.0.7b0/adata/stock/info/
+-rw-rw-rw-   0        0        0      380 2023-05-05 13:46:05.000000 adata-0.0.7b0/adata/stock/info/__init__.py
+-rw-rw-rw-   0        0        0     2550 2023-04-25 15:29:33.000000 adata-0.0.7b0/adata/stock/info/stock_code.py
+-rw-rw-rw-   0        0        0     6722 2023-05-05 14:49:14.000000 adata-0.0.7b0/adata/stock/info/stock_concept.py
+-rw-rw-rw-   0        0        0     2027 2023-05-05 14:11:27.000000 adata-0.0.7b0/adata/stock/info/trade_calendar.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:09:54.402910 adata-0.0.7b0/adata/stock/market/
+-rw-rw-rw-   0        0        0      408 2023-04-13 14:47:15.000000 adata-0.0.7b0/adata/stock/market/__init__.py
+-rw-rw-rw-   0        0        0     2941 2023-04-20 13:03:47.000000 adata-0.0.7b0/adata/stock/market/stock_dividend.py
+-rw-rw-rw-   0        0        0    10485 2023-04-25 15:43:53.000000 adata-0.0.7b0/adata/stock/market/stock_market.py
+-rw-rw-rw-   0        0        0     8363 2023-04-25 15:49:26.000000 adata-0.0.7b0/adata/stock/market/stock_market_concept.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:09:54.404912 adata-0.0.7b0/adata/stock/sentiment/
+-rw-rw-rw-   0        0        0      115 2023-04-06 11:14:06.000000 adata-0.0.7b0/adata/stock/sentiment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:09:54.320912 adata-0.0.7b0/adata.egg-info/
+-rw-rw-rw-   0        0        0     7151 2023-05-05 15:09:54.000000 adata-0.0.7b0/adata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1056 2023-05-05 15:09:54.000000 adata-0.0.7b0/adata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 15:09:54.000000 adata-0.0.7b0/adata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-05-05 15:09:54.000000 adata-0.0.7b0/adata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-05 15:09:54.000000 adata-0.0.7b0/adata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-05-05 13:46:05.000000 adata-0.0.7b0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 15:09:54.408912 adata-0.0.7b0/setup.cfg
+-rw-rw-rw-   0        0        0     1819 2023-05-05 15:09:50.000000 adata-0.0.7b0/setup.py
```

### Comparing `adata-0.0.6b0/LICENSE` & `adata-0.0.7b0/LICENSE`

 * *Files identical despite different names*

### Comparing `adata-0.0.6b0/PKG-INFO` & `adata-0.0.7b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adata
-Version: 0.0.6b0
+Version: 0.0.7b0
 Summary: A Data,A Stock,ETF,Bond,Quant
 Home-page: https://gitee.com/inchaos/adata
 Author: 1nchaos
 Author-email: 9527@1nchaos.com
 License: Apache License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `adata-0.0.6b0/README.md` & `adata-0.0.7b0/README.md`

 * *Files identical despite different names*

### Comparing `adata-0.0.6b0/adata/__init__.py` & `adata-0.0.7b0/adata/__init__.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.6b0/adata/__version__.py` & `adata-0.0.7b0/adata/__version__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-VERSION = (0, 0, 6)
+VERSION = (0, 0, 7)
 # PRERELEASE = None  # alpha, beta or rc
 PRERELEASE = 'beta'  # alpha, beta or rc
 REVISION = None
 
 
 def generate_version(version, prerelease=None, revision=None):
     version_parts = [".".join(map(str, version))]
```

### Comparing `adata-0.0.6b0/adata/common/headers/baidu_headers.py` & `adata-0.0.7b0/adata/common/headers/baidu_headers.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.6b0/adata/common/headers/sina_headers.py` & `adata-0.0.7b0/adata/common/headers/sina_headers.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.6b0/adata/common/headers/ths_headers.py` & `adata-0.0.7b0/adata/common/headers/ths_headers.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.6b0/adata/common/utils/cookie.py` & `adata-0.0.7b0/adata/common/utils/cookie.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.6b0/adata/common/utils/snowflake.py` & `adata-0.0.7b0/adata/common/utils/snowflake.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.6b0/adata/common/utils/sunrequests.py` & `adata-0.0.7b0/adata/common/utils/sunrequests.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.6b0/adata/stock/info/stock_code.py` & `adata-0.0.7b0/adata/stock/info/stock_code.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.6b0/adata/stock/info/stock_concept.py` & `adata-0.0.7b0/adata/stock/info/stock_concept.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.6b0/adata/stock/info/trade_calendar.py` & `adata-0.0.7b0/adata/stock/info/trade_calendar.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.6b0/adata/stock/market/stock_dividend.py` & `adata-0.0.7b0/adata/stock/market/stock_dividend.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.6b0/adata/stock/market/stock_market.py` & `adata-0.0.7b0/adata/stock/market/stock_market.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.6b0/adata/stock/market/stock_market_concept.py` & `adata-0.0.7b0/adata/stock/market/stock_market_concept.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.6b0/adata.egg-info/PKG-INFO` & `adata-0.0.7b0/adata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adata
-Version: 0.0.6b0
+Version: 0.0.7b0
 Summary: A Data,A Stock,ETF,Bond,Quant
 Home-page: https://gitee.com/inchaos/adata
 Author: 1nchaos
 Author-email: 9527@1nchaos.com
 License: Apache License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `adata-0.0.6b0/adata.egg-info/SOURCES.txt` & `adata-0.0.7b0/adata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adata-0.0.6b0/setup.py` & `adata-0.0.7b0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     readme = f.read()
 
 requires = [
     "tqdm~=4.65.0",
     "requests~=2.26.0",
     "pandas~=1.5.3",
     "beautifulsoup4~=4.11.2",
+    "py_mini_racer~=0.6.0",
 ]
 
 
 def setup_package():
     metadata = dict(
         name=about["__title__"],
         version=about["__version__"],
```

