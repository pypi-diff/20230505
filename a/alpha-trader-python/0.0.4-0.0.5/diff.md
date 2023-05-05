# Comparing `tmp/alpha_trader_python-0.0.4.tar.gz` & `tmp/alpha_trader_python-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpha_trader_python-0.0.4.tar", max compression
+gzip compressed data, was "alpha_trader_python-0.0.5.tar", max compression
```

## Comparing `alpha_trader_python-0.0.4.tar` & `alpha_trader_python-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      255 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/README.md
--rw-r--r--   0        0        0       22 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/__init__.py
--rw-r--r--   0        0        0     2074 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/achievement/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/authentication/__init__.py
--rw-r--r--   0        0        0      529 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/bank_account/__init__.py
--rw-r--r--   0        0        0     5117 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/bonds/__init__.py
--rw-r--r--   0        0        0     7987 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/client/__init__.py
--rw-r--r--   0        0        0     3002 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/company/__init__.py
--rw-r--r--   0        0        0      776 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/filter/__init__.py
--rw-r--r--   0        0        0     1155 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/listing/__init__.py
--rw-r--r--   0        0        0      387 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/logging/__init__.py
--rw-r--r--   0        0        0     4276 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/miner/__init__.py
--rw-r--r--   0        0        0     5904 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/order/__init__.py
--rw-r--r--   0        0        0      470 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/owner/__init__.py
--rw-r--r--   0        0        0       71 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/partner/__init__.py
--rw-r--r--   0        0        0     1629 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/portfolio/__init__.py
--rw-r--r--   0        0        0     1895 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/portfolio/position.py
--rw-r--r--   0        0        0        0 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/price/__init__.py
--rw-r--r--   0        0        0      405 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/price/price.py
--rw-r--r--   0        0        0     2790 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/price/price_spread.py
--rw-r--r--   0        0        0     2771 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/securities_account/__init__.py
--rw-r--r--   0        0        0     7727 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/alpha_trader/user/__init__.py
--rw-r--r--   0        0        0      922 2023-05-05 06:55:12.343753 alpha_trader_python-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 alpha_trader_python-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      255 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/README.md
+-rw-r--r--   0        0        0       22 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/__init__.py
+-rw-r--r--   0        0        0     2074 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/achievement/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/authentication/__init__.py
+-rw-r--r--   0        0        0      529 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/bank_account/__init__.py
+-rw-r--r--   0        0        0     5117 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/bonds/__init__.py
+-rw-r--r--   0        0        0     8445 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/client/__init__.py
+-rw-r--r--   0        0        0     3002 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/company/__init__.py
+-rw-r--r--   0        0        0      776 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/filter/__init__.py
+-rw-r--r--   0        0        0     1155 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/listing/__init__.py
+-rw-r--r--   0        0        0      387 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/logging/__init__.py
+-rw-r--r--   0        0        0     4276 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/miner/__init__.py
+-rw-r--r--   0        0        0     6087 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/order/__init__.py
+-rw-r--r--   0        0        0      470 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/owner/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/partner/__init__.py
+-rw-r--r--   0        0        0     1629 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/portfolio/__init__.py
+-rw-r--r--   0        0        0     1895 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/portfolio/position.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/price/__init__.py
+-rw-r--r--   0        0        0      405 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/price/price.py
+-rw-r--r--   0        0        0     2790 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/price/price_spread.py
+-rw-r--r--   0        0        0     2771 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/securities_account/__init__.py
+-rw-r--r--   0        0        0     7727 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/user/__init__.py
+-rw-r--r--   0        0        0      922 2023-05-05 07:31:55.545038 alpha_trader_python-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 alpha_trader_python-0.0.5/PKG-INFO
```

### Comparing `alpha_trader_python-0.0.4/alpha_trader/achievement/__init__.py` & `alpha_trader_python-0.0.5/alpha_trader/achievement/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.4/alpha_trader/bank_account/__init__.py` & `alpha_trader_python-0.0.5/alpha_trader/bank_account/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.4/alpha_trader/bonds/__init__.py` & `alpha_trader_python-0.0.5/alpha_trader/bonds/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.4/alpha_trader/client/__init__.py` & `alpha_trader_python-0.0.5/alpha_trader/client/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     from alpha_trader.miner import Miner
     from alpha_trader.listing import Listing
     from alpha_trader.price.price_spread import PriceSpread
     from alpha_trader.user import User
     from alpha_trader.securities_account import SecuritiesAccount
     from alpha_trader.bonds import Bond
     from alpha_trader.company import Company
+    from alpha_trader.order import Order
 
 from alpha_trader.logging import logger
 
 
 class Client(BaseModel):
     """
     Client for interacting with the Alpha Trader API.
@@ -255,9 +256,25 @@
         """
         from alpha_trader.company import Company
 
         response = self.request("GET", f"api/companies/securityIdentifier/{security_identifier}")
 
         return Company.initialize_from_api_response(response.json(), client=self)
 
+    def get_order(self, order_id: str) -> Order:
+        """
+            Get the order information for a given order ID.
+
+        Args:
+            order_id: Order ID
+
+        Returns:
+            Order
+        """
+        from alpha_trader.order import Order
+
+        response = self.request("GET", f"api/securityorders//{order_id}")
+
+        return Order.initialize_from_api_response(response.json(), client=self)
+
     def get_bonds(self, page: int, search: str, page_size: int):
         pass
```

### Comparing `alpha_trader_python-0.0.4/alpha_trader/company/__init__.py` & `alpha_trader_python-0.0.5/alpha_trader/company/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.4/alpha_trader/filter/__init__.py` & `alpha_trader_python-0.0.5/alpha_trader/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.4/alpha_trader/listing/__init__.py` & `alpha_trader_python-0.0.5/alpha_trader/listing/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.4/alpha_trader/miner/__init__.py` & `alpha_trader_python-0.0.5/alpha_trader/miner/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.4/alpha_trader/order/__init__.py` & `alpha_trader_python-0.0.5/alpha_trader/order/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,19 @@
             "hourlyChange": hourly_change,
         }
 
         response = client.request("POST", "api/securityorders", data=data)
 
         return Order.initialize_from_api_response(response.json(), client)
 
+    def update(self):
+        response = self.client.request("GET", f"api/securityorders/{self.id}")
+
+        return Order.initialize_from_api_response(response.json(), self.client)
+
     def __str__(self):
         return (
             f"{self.action} {self.number_of_shares} {self.listing.name} @ {self.price}"
         )
 
     def __repr__(self):
         return self.__str__()
```

### Comparing `alpha_trader_python-0.0.4/alpha_trader/portfolio/__init__.py` & `alpha_trader_python-0.0.5/alpha_trader/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.4/alpha_trader/portfolio/position.py` & `alpha_trader_python-0.0.5/alpha_trader/portfolio/position.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.4/alpha_trader/price/price_spread.py` & `alpha_trader_python-0.0.5/alpha_trader/price/price_spread.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.4/alpha_trader/securities_account/__init__.py` & `alpha_trader_python-0.0.5/alpha_trader/securities_account/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.4/alpha_trader/user/__init__.py` & `alpha_trader_python-0.0.5/alpha_trader/user/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.4/pyproject.toml` & `alpha_trader_python-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alpha-trader-python"
-version = "0.0.4"
+version = "0.0.5"
 description = "Python SDK for https://alpha-trader.com"
 authors = ["maltemelzer"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "alpha_trader"}]
 
 [tool.poetry.dependencies]
```

### Comparing `alpha_trader_python-0.0.4/PKG-INFO` & `alpha_trader_python-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpha-trader-python
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python SDK for https://alpha-trader.com
 License: MIT
 Author: maltemelzer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

