# Comparing `tmp/vcsc_data_common-0.1.4.tar.gz` & `tmp/vcsc_data_common-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcsc_data_common-0.1.4.tar", last modified: Thu May  4 06:36:44 2023, max compression
+gzip compressed data, was "vcsc_data_common-0.1.5.tar", last modified: Fri May  5 07:00:02 2023, max compression
```

## Comparing `vcsc_data_common-0.1.4.tar` & `vcsc_data_common-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-04 06:36:44.037602 vcsc_data_common-0.1.4/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-05-04 06:36:44.037682 vcsc_data_common-0.1.4/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.1.4/README.md
--rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.1.4/pyproject.toml
--rw-r--r--   0 pd         (501) staff       (20)      339 2023-05-04 06:36:44.037976 vcsc_data_common-0.1.4/setup.cfg
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-04 06:36:44.034777 vcsc_data_common-0.1.4/vcsc_data_common/
--rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.1.4/vcsc_data_common/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-04 06:36:44.036155 vcsc_data_common-0.1.4/vcsc_data_common/ai_framework/
--rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.1.4/vcsc_data_common/ai_framework/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     4948 2023-03-31 09:44:29.000000 vcsc_data_common-0.1.4/vcsc_data_common/ai_framework/interval_fetching.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-04 06:36:44.036480 vcsc_data_common-0.1.4/vcsc_data_common/live_price_data/
--rw-r--r--   0 pd         (501) staff       (20)     2341 2023-05-04 06:36:10.000000 vcsc_data_common-0.1.4/vcsc_data_common/live_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-04 06:36:44.036779 vcsc_data_common-0.1.4/vcsc_data_common/offline_price_data/
--rw-r--r--   0 pd         (501) staff       (20)      880 2023-03-14 02:58:59.000000 vcsc_data_common-0.1.4/vcsc_data_common/offline_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-04 06:36:44.037066 vcsc_data_common-0.1.4/vcsc_data_common/order/
--rw-r--r--   0 pd         (501) staff       (20)     3647 2023-03-27 04:29:07.000000 vcsc_data_common-0.1.4/vcsc_data_common/order/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-04 06:36:44.037358 vcsc_data_common-0.1.4/vcsc_data_common/portfolio_info/
--rw-r--r--   0 pd         (501) staff       (20)     3444 2023-04-21 06:19:05.000000 vcsc_data_common-0.1.4/vcsc_data_common/portfolio_info/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-04 06:36:44.035681 vcsc_data_common-0.1.4/vcsc_data_common.egg-info/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-05-04 06:36:44.000000 vcsc_data_common-0.1.4/vcsc_data_common.egg-info/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      527 2023-05-04 06:36:44.000000 vcsc_data_common-0.1.4/vcsc_data_common.egg-info/SOURCES.txt
--rw-r--r--   0 pd         (501) staff       (20)        1 2023-05-04 06:36:44.000000 vcsc_data_common-0.1.4/vcsc_data_common.egg-info/dependency_links.txt
--rw-r--r--   0 pd         (501) staff       (20)      140 2023-05-04 06:36:44.000000 vcsc_data_common-0.1.4/vcsc_data_common.egg-info/requires.txt
--rw-r--r--   0 pd         (501) staff       (20)       17 2023-05-04 06:36:44.000000 vcsc_data_common-0.1.4/vcsc_data_common.egg-info/top_level.txt
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-05 07:00:02.378660 vcsc_data_common-0.1.5/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-05-05 07:00:02.378763 vcsc_data_common-0.1.5/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.1.5/README.md
+-rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.1.5/pyproject.toml
+-rw-r--r--   0 pd         (501) staff       (20)      339 2023-05-05 07:00:02.379138 vcsc_data_common-0.1.5/setup.cfg
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-05 07:00:02.375260 vcsc_data_common-0.1.5/vcsc_data_common/
+-rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.1.5/vcsc_data_common/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-05 07:00:02.377243 vcsc_data_common-0.1.5/vcsc_data_common/ai_framework/
+-rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.1.5/vcsc_data_common/ai_framework/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     4948 2023-03-31 09:44:29.000000 vcsc_data_common-0.1.5/vcsc_data_common/ai_framework/interval_fetching.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-05 07:00:02.377531 vcsc_data_common-0.1.5/vcsc_data_common/live_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)     2341 2023-05-04 06:36:10.000000 vcsc_data_common-0.1.5/vcsc_data_common/live_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-05 07:00:02.377834 vcsc_data_common-0.1.5/vcsc_data_common/offline_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)      880 2023-03-14 02:58:59.000000 vcsc_data_common-0.1.5/vcsc_data_common/offline_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-05 07:00:02.378116 vcsc_data_common-0.1.5/vcsc_data_common/order/
+-rw-r--r--   0 pd         (501) staff       (20)     3647 2023-03-27 04:29:07.000000 vcsc_data_common-0.1.5/vcsc_data_common/order/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-05 07:00:02.378405 vcsc_data_common-0.1.5/vcsc_data_common/portfolio_info/
+-rw-r--r--   0 pd         (501) staff       (20)     3476 2023-05-05 06:59:07.000000 vcsc_data_common-0.1.5/vcsc_data_common/portfolio_info/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-05 07:00:02.376747 vcsc_data_common-0.1.5/vcsc_data_common.egg-info/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-05-05 07:00:02.000000 vcsc_data_common-0.1.5/vcsc_data_common.egg-info/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      527 2023-05-05 07:00:02.000000 vcsc_data_common-0.1.5/vcsc_data_common.egg-info/SOURCES.txt
+-rw-r--r--   0 pd         (501) staff       (20)        1 2023-05-05 07:00:02.000000 vcsc_data_common-0.1.5/vcsc_data_common.egg-info/dependency_links.txt
+-rw-r--r--   0 pd         (501) staff       (20)      140 2023-05-05 07:00:02.000000 vcsc_data_common-0.1.5/vcsc_data_common.egg-info/requires.txt
+-rw-r--r--   0 pd         (501) staff       (20)       17 2023-05-05 07:00:02.000000 vcsc_data_common-0.1.5/vcsc_data_common.egg-info/top_level.txt
```

### Comparing `vcsc_data_common-0.1.4/pyproject.toml` & `vcsc_data_common-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.4/vcsc_data_common/ai_framework/interval_fetching.py` & `vcsc_data_common-0.1.5/vcsc_data_common/ai_framework/interval_fetching.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.4/vcsc_data_common/live_price_data/__init__.py` & `vcsc_data_common-0.1.5/vcsc_data_common/live_price_data/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.4/vcsc_data_common/offline_price_data/__init__.py` & `vcsc_data_common-0.1.5/vcsc_data_common/offline_price_data/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.4/vcsc_data_common/order/__init__.py` & `vcsc_data_common-0.1.5/vcsc_data_common/order/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.4/vcsc_data_common/portfolio_info/__init__.py` & `vcsc_data_common-0.1.5/vcsc_data_common/portfolio_info/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
             select t1."portfolioConfigId",t4."tradingModel",t4."portfolioModel",t1.username,t1.symbol,COALESCE("latestMatchPrice",0) as "latestMatchPrice",
                 "totalAmount",CASE WHEN "forceSellAmount" > "availableAmount" THEN 0 ELSE "availableAmount" - "forceSellAmount"  END as "availableAmount",
                 "scheduledAmount", "averageMatchedPrice","targetPercent",
                 "balance","initBalance", t1."cutoffDate", "forceSellAmount" , t1."portfolioType"
                 from "portfolio" t1
                 left join "symbol_info" t2 on t1.symbol = t2.symbol
                 left join "portfolio_config" t4 on t1."portfolioConfigId" = t4.id
+				WHERE t4.status = 'RUNNING'
         """, con=self.paper_trading_db_connection)
 
     def update_target_percent_portfolio(self, portfolio_data: dict, cycle_length: int, portfolioModel: int):
 
         url = f"{self.paper_trading_api_end_point}/portfolioRatio/updateNewRatio"
 
         payload = json.dumps({
```

### Comparing `vcsc_data_common-0.1.4/vcsc_data_common.egg-info/SOURCES.txt` & `vcsc_data_common-0.1.5/vcsc_data_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

