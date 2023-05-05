# Comparing `tmp/alpha_trader_python-0.0.2.tar.gz` & `tmp/alpha_trader_python-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpha_trader_python-0.0.2.tar", max compression
+gzip compressed data, was "alpha_trader_python-0.0.3.tar", max compression
```

## Comparing `alpha_trader_python-0.0.2.tar` & `alpha_trader_python-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      255 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/README.md
--rw-r--r--   0        0        0       22 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/__init__.py
--rw-r--r--   0        0        0     2074 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/achievement/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/authentication/__init__.py
--rw-r--r--   0        0        0      529 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/bank_account/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/bonds/__init__.py
--rw-r--r--   0        0        0     7460 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/client/__init__.py
--rw-r--r--   0        0        0     2993 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/company/__init__.py
--rw-r--r--   0        0        0      776 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/filter/__init__.py
--rw-r--r--   0        0        0     1155 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/listing/__init__.py
--rw-r--r--   0        0        0      387 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/logging/__init__.py
--rw-r--r--   0        0        0     4276 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/miner/__init__.py
--rw-r--r--   0        0        0     5904 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/order/__init__.py
--rw-r--r--   0        0        0      470 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/owner/__init__.py
--rw-r--r--   0        0        0       71 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/partner/__init__.py
--rw-r--r--   0        0        0     1629 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/portfolio/__init__.py
--rw-r--r--   0        0        0     1895 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/portfolio/position.py
--rw-r--r--   0        0        0        0 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/price/__init__.py
--rw-r--r--   0        0        0      405 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/price/price.py
--rw-r--r--   0        0        0     2790 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/price/price_spread.py
--rw-r--r--   0        0        0     2771 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/securities_account/__init__.py
--rw-r--r--   0        0        0     7727 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/user/__init__.py
--rw-r--r--   0        0        0      922 2023-05-04 06:59:39.911919 alpha_trader_python-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 alpha_trader_python-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      255 2023-05-04 07:36:03.836244 alpha_trader_python-0.0.3/README.md
+-rw-r--r--   0        0        0       22 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/__init__.py
+-rw-r--r--   0        0        0     2074 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/achievement/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/authentication/__init__.py
+-rw-r--r--   0        0        0      529 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/bank_account/__init__.py
+-rw-r--r--   0        0        0     5117 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/bonds/__init__.py
+-rw-r--r--   0        0        0     7460 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/client/__init__.py
+-rw-r--r--   0        0        0     3002 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/company/__init__.py
+-rw-r--r--   0        0        0      776 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/filter/__init__.py
+-rw-r--r--   0        0        0     1155 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/listing/__init__.py
+-rw-r--r--   0        0        0      387 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/logging/__init__.py
+-rw-r--r--   0        0        0     4276 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/miner/__init__.py
+-rw-r--r--   0        0        0     5904 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/order/__init__.py
+-rw-r--r--   0        0        0      470 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/owner/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/partner/__init__.py
+-rw-r--r--   0        0        0     1629 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/portfolio/__init__.py
+-rw-r--r--   0        0        0     1895 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/portfolio/position.py
+-rw-r--r--   0        0        0        0 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/price/__init__.py
+-rw-r--r--   0        0        0      405 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/price/price.py
+-rw-r--r--   0        0        0     2790 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/price/price_spread.py
+-rw-r--r--   0        0        0     2771 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/securities_account/__init__.py
+-rw-r--r--   0        0        0     7727 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/alpha_trader/user/__init__.py
+-rw-r--r--   0        0        0      922 2023-05-04 07:36:03.840244 alpha_trader_python-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 alpha_trader_python-0.0.3/PKG-INFO
```

### Comparing `alpha_trader_python-0.0.2/alpha_trader/achievement/__init__.py` & `alpha_trader_python-0.0.3/alpha_trader/achievement/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.2/alpha_trader/bank_account/__init__.py` & `alpha_trader_python-0.0.3/alpha_trader/bank_account/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.2/alpha_trader/bonds/__init__.py` & `alpha_trader_python-0.0.3/alpha_trader/bonds/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,37 +4,46 @@
 from typing import Dict, TYPE_CHECKING, Union
 import time
 
 # if TYPE_CHECKING:
 from alpha_trader.client import Client
 from alpha_trader.listing import Listing
 from alpha_trader.price.price_spread import PriceSpread
+from alpha_trader.company import Company
 
 
 class Issuer(BaseModel):
     id: str
     # listing: Listing
     name: str
     security_identifier: str
     version: int
+    client: Client
 
     @staticmethod
-    def initialize_from_api_response(api_response: Dict) -> "Issuer":
+    def initialize_from_api_response(api_response: Dict, client: Client) -> "Issuer":
         # from alpha_trader.listing import Listing
 
         return Issuer(
             id=api_response["id"],
             # listing=Listing.initialize_from_api_response(
             #     api_response["listing"], client
             # ),
             name=api_response["name"],
             security_identifier=api_response["securityIdentifier"],
             version=api_response["version"],
+            client=client,
         )
 
+    @property
+    def company(self):
+        response = self.client.request("GET", f"api/companies/securityIdentifier/{self.security_identifier}")
+
+        return Company.initialize_from_api_response(response.json(), self.client)
+
 
 class Bond(BaseModel):
     """
         Bond security.
 
         Attributes:
             face_value: Face value of the bond.
@@ -74,15 +83,15 @@
             price_spread = PriceSpread.initialize_from_api_response(api_response["priceSpread"], client)
 
         return Bond(
             face_value=api_response["faceValue"],
             id=api_response["id"],
             interest_rate=api_response["interestRate"],
             issue_date=api_response["issueDate"],
-            issuer=Issuer.initialize_from_api_response(api_response["issuer"]),
+            issuer=Issuer.initialize_from_api_response(api_response["issuer"], client=client),
             listing=Listing.initialize_from_api_response(api_response["listing"], client),
             maturity_date=api_response["maturityDate"],
             name=api_response["name"],
             price_spread=price_spread,
             repurchase_listing=Listing.initialize_from_api_response(api_response["repurchaseListing"], client),
             version=api_response["version"],
             volume=api_response["volume"],
```

### Comparing `alpha_trader_python-0.0.2/alpha_trader/client/__init__.py` & `alpha_trader_python-0.0.3/alpha_trader/client/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.2/alpha_trader/company/__init__.py` & `alpha_trader_python-0.0.3/alpha_trader/company/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from pydantic import BaseModel
 from typing import Dict
 
 from alpha_trader.client import Client
 from alpha_trader.listing import Listing
 from alpha_trader.bank_account import BankAccount
-from alpha_trader.bonds import Bond
 from alpha_trader.user import User
 
 
 class Company(BaseModel):
     achievement_count: int
     achievement_count: int
     bank_account: BankAccount
@@ -77,14 +76,16 @@
     def issue_bonds(
             self,
             face_value: float,
             interest_rate: float,
             maturity_date: int,
             number_of_bonds: int
     ):
+        from alpha_trader.bonds import Bond
+
         return Bond.issue(
             self.id,
             face_value=face_value,
             interest_rate=interest_rate,
             maturity_date=maturity_date,
             number_of_bonds=number_of_bonds,
             client=self.client
```

### Comparing `alpha_trader_python-0.0.2/alpha_trader/filter/__init__.py` & `alpha_trader_python-0.0.3/alpha_trader/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.2/alpha_trader/listing/__init__.py` & `alpha_trader_python-0.0.3/alpha_trader/listing/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.2/alpha_trader/miner/__init__.py` & `alpha_trader_python-0.0.3/alpha_trader/miner/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.2/alpha_trader/order/__init__.py` & `alpha_trader_python-0.0.3/alpha_trader/order/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.2/alpha_trader/portfolio/__init__.py` & `alpha_trader_python-0.0.3/alpha_trader/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.2/alpha_trader/portfolio/position.py` & `alpha_trader_python-0.0.3/alpha_trader/portfolio/position.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.2/alpha_trader/price/price_spread.py` & `alpha_trader_python-0.0.3/alpha_trader/price/price_spread.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.2/alpha_trader/securities_account/__init__.py` & `alpha_trader_python-0.0.3/alpha_trader/securities_account/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.2/alpha_trader/user/__init__.py` & `alpha_trader_python-0.0.3/alpha_trader/user/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.2/pyproject.toml` & `alpha_trader_python-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alpha-trader-python"
-version = "0.0.2"
+version = "0.0.3"
 description = "Python SDK for https://alpha-trader.com"
 authors = ["maltemelzer"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "alpha_trader"}]
 
 [tool.poetry.dependencies]
```

### Comparing `alpha_trader_python-0.0.2/PKG-INFO` & `alpha_trader_python-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpha-trader-python
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python SDK for https://alpha-trader.com
 License: MIT
 Author: maltemelzer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

