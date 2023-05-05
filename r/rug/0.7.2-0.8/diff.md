# Comparing `tmp/rug-0.7.2.tar.gz` & `tmp/rug-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rug-0.7.2.tar", max compression
+gzip compressed data, was "rug-0.8.tar", max compression
```

## Comparing `rug-0.7.2.tar` & `rug-0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      775 2022-12-23 18:16:50.519949 rug-0.7.2/README.md
--rw-r--r--   0        0        0      868 2023-03-23 14:18:39.588416 rug-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      288 2022-12-15 16:02:47.957044 rug-0.7.2/rug/__init__.py
--rw-r--r--   0        0        0     4266 2022-10-10 19:45:59.707606 rug-0.7.2/rug/alphaquery.py
--rw-r--r--   0        0        0     2688 2022-08-11 07:37:52.820634 rug-0.7.2/rug/barchart.py
--rw-r--r--   0        0        0     4641 2022-12-15 16:08:39.724843 rug-0.7.2/rug/base.py
--rw-r--r--   0        0        0     4150 2022-12-23 18:09:17.774153 rug-0.7.2/rug/etfdb.py
--rw-r--r--   0        0        0      683 2022-07-27 20:03:36.438856 rug-0.7.2/rug/exceptions.py
--rw-r--r--   0        0        0     1121 2022-08-11 08:41:44.654954 rug-0.7.2/rug/finviz.py
--rw-r--r--   0        0        0     1253 2022-12-12 10:12:35.894849 rug-0.7.2/rug/stockanalysis.py
--rw-r--r--   0        0        0     1947 2022-08-11 08:42:20.047418 rug-0.7.2/rug/stocktwits.py
--rw-r--r--   0        0        0     6640 2023-03-23 14:18:25.484256 rug-0.7.2/rug/tipranks.py
--rw-r--r--   0        0        0     4022 2022-08-11 08:43:03.063984 rug-0.7.2/rug/yahoo.py
--rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 rug-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      775 2022-12-23 18:16:50.519949 rug-0.8/README.md
+-rw-r--r--   0        0        0      851 2023-05-05 07:11:21.747804 rug-0.8/pyproject.toml
+-rw-r--r--   0        0        0      288 2022-12-15 16:02:47.957044 rug-0.8/rug/__init__.py
+-rw-r--r--   0        0        0     4266 2022-10-10 19:45:59.707606 rug-0.8/rug/alphaquery.py
+-rw-r--r--   0        0        0     2688 2022-08-11 07:37:52.820634 rug-0.8/rug/barchart.py
+-rw-r--r--   0        0        0     4641 2022-12-15 16:08:39.724843 rug-0.8/rug/base.py
+-rw-r--r--   0        0        0     4150 2022-12-23 18:09:17.774153 rug-0.8/rug/etfdb.py
+-rw-r--r--   0        0        0      683 2022-07-27 20:03:36.438856 rug-0.8/rug/exceptions.py
+-rw-r--r--   0        0        0     3002 2023-04-05 05:45:36.800863 rug-0.8/rug/finviz.py
+-rw-r--r--   0        0        0     1253 2022-12-12 10:12:35.894849 rug-0.8/rug/stockanalysis.py
+-rw-r--r--   0        0        0     1947 2022-08-11 08:42:20.047418 rug-0.8/rug/stocktwits.py
+-rw-r--r--   0        0        0     6910 2023-05-05 06:58:34.815386 rug-0.8/rug/tipranks.py
+-rw-r--r--   0        0        0     4022 2022-08-11 08:43:03.063984 rug-0.8/rug/yahoo.py
+-rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 rug-0.8/PKG-INFO
```

### Comparing `rug-0.7.2/README.md` & `rug-0.8/README.md`

 * *Files identical despite different names*

### Comparing `rug-0.7.2/pyproject.toml` & `rug-0.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "rug"
-version = "0.7.2"
+version = "0.8"
 description = "Library for fetching various stock data from the internet (official and unofficial APIs)."
-authors = ["Pavel Hrdina, Patrick Roach"]
+authors = ["Pavel Hrdina"]
 classifiers = [
     "Programming Language :: Python :: 3.6",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries",
 ]
```

### Comparing `rug-0.7.2/rug/alphaquery.py` & `rug-0.8/rug/alphaquery.py`

 * *Files identical despite different names*

### Comparing `rug-0.7.2/rug/barchart.py` & `rug-0.8/rug/barchart.py`

 * *Files identical despite different names*

### Comparing `rug-0.7.2/rug/base.py` & `rug-0.8/rug/base.py`

 * *Files identical despite different names*

### Comparing `rug-0.7.2/rug/etfdb.py` & `rug-0.8/rug/etfdb.py`

 * *Files identical despite different names*

### Comparing `rug-0.7.2/rug/exceptions.py` & `rug-0.8/rug/exceptions.py`

 * *Files identical despite different names*

### Comparing `rug-0.7.2/rug/finviz.py` & `rug-0.8/rug/stockanalysis.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 import re
 
 from .base import BaseAPI, HtmlTableParser
-from .exceptions import SymbolNotFound
+from .exceptions import DataException, SymbolNotFound
 
 
-class FinViz(BaseAPI):
-    """
-    FinViz.com
-    """
-
-    def get_price_ratings(self):
+class StockAnalysis(BaseAPI):
+    def get_etf_holdings(self):
         """
-        Returns price ratings a.k.a price targets
-        by analysts.
-
-        Returned rows are:
-
-        - date
-        - status
-        - analyst
-        - rating
-        - target price
+        Fetches ETF holdings table with following columns:
 
-        :return: Rows as a list of tuples where each tuple has 5 items.
-        :rtype: list
+        - No.
+        - Symbol
+        - Name
+        - % Weight
+        - Shares
         """
 
         try:
             html = self._get(
-                f"https://finviz.com/quote.ashx?t={self.symbol.upper()}&ty=c&ta=1&p=d",
-                headers={"User-Agent": self.user_agent},
+                f"https://stockanalysis.com/etf/{self.symbol.lower()}/holdings/"
             )
         except Exception as e:
             raise SymbolNotFound from e
 
-        finds = re.findall(
-            r"<td[^>]*fullview-ratings-inner[^>]*>(<table[^>]*>(?:.+?)<\/table>)",
-            html.text,
-            re.DOTALL,
-        )
-        rows = []
-
-        for find in finds:
-            parser = HtmlTableParser(columns=5)
-            parser.feed(find)
-            rows.extend(parser.get_data())
+        finds = re.findall(r"<table.*?>.*?</table>", html.text, re.DOTALL)
+
+        # Check if the HTML contains only one table.
+        if 0 == len(finds):
+            raise SymbolNotFound
+        if 1 < len(finds):
+            raise DataException(
+                "More that one table found in HTML - don't know what to do now"
+            )
+
+        parser = HtmlTableParser(columns=5)
+        # monkey patch - fixing the case where table header is
+        # improperly parsed  - "%" has it's own column and the
+        # last "shares" column is then not parsed.
+        parser.feed(finds[0])
+        parser.data[:6] = ("No.", "Symbol", "Name", "% Weight", "Shares")
 
-        return rows
+        return parser.get_data()
```

### Comparing `rug-0.7.2/rug/stocktwits.py` & `rug-0.8/rug/stocktwits.py`

 * *Files identical despite different names*

### Comparing `rug-0.7.2/rug/tipranks.py` & `rug-0.8/rug/tipranks.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
         dividends = []
 
         if data["dividend"]["history"]:
             for item in data["dividend"]["history"]:
                 dividends.append(
                     {
-                        "yield": float(item["yield"]),
+                        "yield": float(item["yield"]) * 100,
                         "amount": float(item["amount"]),
                         "ex_date": datetime.strptime(
                             item["executionDate"], "%Y-%m-%dT%H:%M:%S.000Z"
                         ).date()
                         if item["executionDate"]
                         else None,
                         "payment_date": datetime.strptime(
@@ -176,17 +176,24 @@
             - market_cap
 
             :param str symbol: Symbol the data will be downloaded for.
             :return: Dict with data.
             :rtype: dict
             """
 
-            data = await self._aget(
-                f"https://market.tipranks.com/api/details/GetRealTimeQuotes/?tickers={symbol}"
-            )
+            try:
+                data = await self._aget(
+                    f"https://market.tipranks.com/api/details/GetRealTimeQuotes/?tickers={symbol}"
+                )
+            except httpx.HTTPStatusError as e:
+                # Checking if symbol was even found.
+                if 404 == e.response.status_code:
+                    raise SymbolNotFound
+                raise HttpException from e
+
             json_data = data.json()
 
             # Checking if symbol was even found.
             if 0 == len(json_data) or "currency" not in json_data[0]:
                 raise SymbolNotFound
 
             return {
```

### Comparing `rug-0.7.2/rug/yahoo.py` & `rug-0.8/rug/yahoo.py`

 * *Files identical despite different names*

### Comparing `rug-0.7.2/PKG-INFO` & `rug-0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: rug
-Version: 0.7.2
+Version: 0.8
 Summary: Library for fetching various stock data from the internet (official and unofficial APIs).
 Home-page: https://github.com/im-n1/rug
 License: MIT
-Author: Pavel Hrdina, Patrick Roach
+Author: Pavel Hrdina
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

