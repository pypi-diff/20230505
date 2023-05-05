# Comparing `tmp/swedish_market_insights-0.2.3.tar.gz` & `tmp/swedish_market_insights-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swedish_market_insights-0.2.3.tar", max compression
+gzip compressed data, was "swedish_market_insights-0.3.0.tar", max compression
```

## Comparing `swedish_market_insights-0.2.3.tar` & `swedish_market_insights-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1298 2023-05-05 07:58:19.608848 swedish_market_insights-0.2.3/README.md
--rw-r--r--   0        0        0      550 2023-05-05 07:58:19.608848 swedish_market_insights-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-05 07:58:19.608848 swedish_market_insights-0.2.3/swedish_market_insights/__init__.py
--rw-r--r--   0        0        0     2245 2023-05-05 07:58:19.608848 swedish_market_insights-0.2.3/swedish_market_insights/ficlient.py
--rw-r--r--   0        0        0      739 2023-05-05 07:58:19.608848 swedish_market_insights-0.2.3/swedish_market_insights/soup_utils.py
--rw-r--r--   0        0        0     1935 2023-05-05 07:58:19.608848 swedish_market_insights-0.2.3/swedish_market_insights/trade.py
--rw-r--r--   0        0        0      565 2023-05-05 07:58:19.608848 swedish_market_insights-0.2.3/swedish_market_insights/utils.py
--rw-r--r--   0        0        0     2058 1970-01-01 00:00:00.000000 swedish_market_insights-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1856 2023-05-05 11:43:51.794249 swedish_market_insights-0.3.0/README.md
+-rw-r--r--   0        0        0      606 2023-05-05 11:43:51.794249 swedish_market_insights-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-05 11:43:51.794249 swedish_market_insights-0.3.0/swedish_market_insights/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-05 11:43:51.794249 swedish_market_insights-0.3.0/swedish_market_insights/constants.py
+-rw-r--r--   0        0        0     2305 2023-05-05 11:43:51.794249 swedish_market_insights-0.3.0/swedish_market_insights/inside_trades.py
+-rw-r--r--   0        0        0      940 2023-05-05 11:43:51.794249 swedish_market_insights-0.3.0/swedish_market_insights/short_positions.py
+-rw-r--r--   0        0        0      790 2023-05-05 11:43:51.794249 swedish_market_insights-0.3.0/swedish_market_insights/soup_utils.py
+-rw-r--r--   0        0        0      565 2023-05-05 11:43:51.794249 swedish_market_insights-0.3.0/swedish_market_insights/utils.py
+-rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 swedish_market_insights-0.3.0/PKG-INFO
```

### Comparing `swedish_market_insights-0.2.3/pyproject.toml` & `swedish_market_insights-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [tool.poetry]
 name = "swedish_market_insights"
-version = "0.2.3"
+version = "0.3.0"
 description = "Package to scrape the Finansinspektion's registers"
 authors = ["Fritjof Bengtsson <fritjof.folkeson@gmail.com>"]
 repository = "https://github.com/fritjof-b/swedish-market-insights"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 beautifulsoup4 = "^4.12.2"
-requests = "^2.28.2"
+requests = "2.28.2"
+pandas = "^2.0.1"
+odfpy = "^1.4.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.1"
+responses = "^0.23.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `swedish_market_insights-0.2.3/swedish_market_insights/soup_utils.py` & `swedish_market_insights-0.3.0/swedish_market_insights/soup_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from bs4 import BeautifulSoup
+import pandas as pd
 
-from .trade import TradeEntry
 
+def get_trade_entries_from_page(page_content: bytes) -> pd.DataFrame:
+    soup = BeautifulSoup(page_content, "html.parser")
+    table = soup.find("table")
+    rows = table.find_all("tr")
 
-def get_trade_entries_from_page(page: bytes) -> list[TradeEntry]:
-    trade_entries = []
-    soup = BeautifulSoup(page, "html.parser")
-    table_rows = soup.find_all("tr")
-    for row in table_rows[1:]:
-        row_data = [
-            tag.get_text(strip=True).replace("\xa0", " ") for tag in row.find_all("td")
-        ]
-        trade_entries.append(TradeEntry.from_row(row_data))
-    return trade_entries
+    header_row = rows.pop(0)
+    columns = [col.get_text(strip=True) for col in header_row.find_all("th")]
+
+    data = []
+    for row in rows:
+        data.append([col.get_text(strip=True) for col in row.find_all("td")])
+
+    df = pd.DataFrame(data, columns=columns)
+    return df
 
 
 def find_href_for_next_page(page: bytes) -> str:
     soup = BeautifulSoup(page, "html.parser")
     next_button = soup.find("li", class_="next")
     if next_button and next_button.a:
         href = next_button.a.get("href")
```

### Comparing `swedish_market_insights-0.2.3/swedish_market_insights/utils.py` & `swedish_market_insights-0.3.0/swedish_market_insights/utils.py`

 * *Files identical despite different names*

### Comparing `swedish_market_insights-0.2.3/PKG-INFO` & `swedish_market_insights-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,78 +1,95 @@
 Metadata-Version: 2.1
 Name: swedish-market-insights
-Version: 0.2.3
+Version: 0.3.0
 Summary: Package to scrape the Finansinspektion's registers
 Home-page: https://github.com/fritjof-b/swedish-market-insights
 License: MIT
 Author: Fritjof Bengtsson
 Author-email: fritjof.folkeson@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: odfpy (>=1.4.1,<2.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: requests (==2.28.2)
 Project-URL: Repository, https://github.com/fritjof-b/swedish-market-insights
 Description-Content-Type: text/markdown
 
 # Swedish Market Insights
 
 SMI is a small package for fetching inside trades made in Sweden.
-The data is collected with `requests` and parsed with `BeautifulSoup4`.
+The data is collected with `requests` and parsed with `BeautifulSoup4`
+and returned as a `pandas.DataFrame`.
+
 All data is publicly available on Finansinspektionen's [website](https://fi.se/).
 
 ## Installation
 
 ```
-pip install insyn
+pip install swedish-market-insights
 ```
 
 ## Usage
 
 ```python3
-from swedish_market_insights import ficlient
+from swedish_market_insights.inside_trades import InsideTradesAPI
+from swedish_market_insights.short_positions import ShortPositionsAPI
 
-api = ficlient.FiClient()
-recent_inside_trades = api.get_trades_by_transaction_date()
+recent_inside_trades = InsideTradesAPI.get_trades_by_transaction_date()
+current_short_positions = ShortPositionsAPI.get_current_short_positions()
 ```
 
 ## Features
 
+### Inside Trades
 - Fetch inside trades by transaction date
 - Fetch inside trades by publication date
 
+### Short Positions
+- Fetch current short positions
+- Fetch historical short positions
+- Fetch aggregated short positions
+
 ## Examples
 
 ### Fetch inside trades by transaction date
 
 ```python3
-from swedish_market_insights import ficlient
+from swedish_market_insights.inside_trades import InsideTradesAPI
 from datetime import date
 
-api = ficlient.FiClient()
-trades = api.get_trades_by_transaction_date(
+trades = InsideTradesAPI.get_trades_by_transaction_date(
     from_date=date(2020, 1, 1),
     to_date=date(2020, 1, 31))
 ```
 
 ### Fetch inside trades by publication date
 
 ```python3
+from swedish_market_insights.inside_trades import InsideTradesAPI
 from datetime import date
-from swedish_market_insights import ficlient
 
-api = ficlient.FiClient()
-trades = api.get_trades_by_publish_date(
+trades = InsideTradesAPI.get_trades_by_publish_date(
     from_date=date(2022, 10, 8),
     to_date=date(2022, 10, 10))
 ```
 
+### Fetch current short positions
+
+```python3
+from swedish_market_insights.short_positions import ShortPositionsAPI
+
+current_short_positions = ShortPositionsAPI.get_current_short_positions()
+```
+
 ## Contributing
 
 Contributions are welcome! Please open an issue or submit a pull request on GitHub if you have any suggestions or
 improvements.
 
 ## License
```

