# Comparing `tmp/findmyorder-1.2.4.tar.gz` & `tmp/findmyorder-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.2.4.tar", max compression
+gzip compressed data, was "findmyorder-1.3.0.tar", max compression
```

## Comparing `findmyorder-1.2.4.tar` & `findmyorder-1.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-04 19:16:22.429576 findmyorder-1.2.4/LICENSE
--rw-r--r--   0        0        0     2156 2023-05-04 19:16:22.429576 findmyorder-1.2.4/README.md
--rw-r--r--   0        0        0      113 2023-05-04 19:16:23.117590 findmyorder-1.2.4/findmyorder/__init__.py
--rw-r--r--   0        0        0      631 2023-05-04 19:16:22.429576 findmyorder-1.2.4/findmyorder/config.py
--rw-r--r--   0        0        0      566 2023-05-04 19:16:22.429576 findmyorder-1.2.4/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     4031 2023-05-04 19:16:22.429576 findmyorder-1.2.4/findmyorder/main.py
--rw-r--r--   0        0        0     1758 2023-05-04 19:16:23.117590 findmyorder-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     2976 1970-01-01 00:00:00.000000 findmyorder-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-05 18:47:08.248635 findmyorder-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2155 2023-05-05 18:47:08.248635 findmyorder-1.3.0/README.md
+-rw-r--r--   0        0        0      113 2023-05-05 18:47:08.996644 findmyorder-1.3.0/findmyorder/__init__.py
+-rw-r--r--   0        0        0      631 2023-05-05 18:47:08.248635 findmyorder-1.3.0/findmyorder/config.py
+-rw-r--r--   0        0        0      566 2023-05-05 18:47:08.248635 findmyorder-1.3.0/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     4127 2023-05-05 18:47:08.248635 findmyorder-1.3.0/findmyorder/main.py
+-rw-r--r--   0        0        0     1758 2023-05-05 18:47:08.996644 findmyorder-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 findmyorder-1.3.0/PKG-INFO
```

### Comparing `findmyorder-1.2.4/LICENSE` & `findmyorder-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.2.4/README.md` & `findmyorder-1.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 
 | <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"> | A python package to identify and parse order for trade execution. |
 | ------------- | ------------- |
 |[![Pypi](https://badgen.net/badge/icon/findmyorder?icon=pypi&label)](https://pypi.org/project/findmyorder/) ![Version](https://img.shields.io/pypi/v/findmyorder)<br>  ![Pypi](https://img.shields.io/pypi/dm/findmyorder)<br> [![Build](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/findmyorder/branch/dev/graph/badge.svg?token=4838MSZNCC)](https://codecov.io/gh/mraniki/findmyorder) | Find & Parse a trade order for execution|
 
 
-
 Key features:
 
 - Identify an order with word `BUY SELL LONG SHORT` or your own `Bull`, `to the moon`, `pump` via config file
 - Parse and return a structured order with action and instrument as mandatory
 - Settings for custom option
```

### Comparing `findmyorder-1.2.4/findmyorder/config.py` & `findmyorder-1.3.0/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.2.4/findmyorder/default_settings.toml` & `findmyorder-1.3.0/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.2.4/findmyorder/main.py` & `findmyorder-1.3.0/findmyorder/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """
  FindMyOrder Main
 """
 import logging
-from datetime import datetime, timezone
+from datetime import datetime
 
 from pyparsing import Combine, Optional, Word, alphas, nums, one_of, pyparsing_common,  Suppress
 
 from .config import settings
 
+
 class FindMyOrder:
     """find an order class """
 
     def __init__(
         self,
     ):
         self.logger = logging.getLogger(__name__)
 
     async def search(
         self,
         mystring: str,
-    )-> bool:
+    ) -> bool:
         """Search an order."""
         try:
             logging.info(mystring)
             string_check = mystring.split()[0]
             logging.info("action identifier %s", settings.action_identifier)
             if string_check.lower() in settings.action_identifier.lower():
                 logging.debug("found order in %s ", mystring)
@@ -33,54 +34,59 @@
         except Exception as e:
             logging.warning("SearchError: %s", e)
             return False
 
     async def identify_order(
             self,
             mystring: str,
-        ) -> dict:
+            ) -> dict:
         """Identify an order."""
         logging.debug("identify_order: %s", mystring)
         try:
             action = one_of(
                 settings.action_identifier, caseless=True
                 ).set_results_name("action").set_parse_action(pyparsing_common.upcase_tokens)
             instrument = Word(
                 alphas
                 ).set_results_name("instrument")
             stop_loss = Combine(
-                    Suppress(settings.stop_loss_identifier) + Word(nums)
+                    Suppress(settings.stop_loss_identifier) 
+                    + Word(nums)
                 ).set_results_name("stop_loss")
             take_profit = Combine(
-                Suppress(settings.take_profit_identifier) + Word(nums)
+                Suppress(settings.take_profit_identifier) 
+                + Word(nums)
                 ).set_results_name("take_profit")
             quantity = Combine(
-                Suppress(settings.quantity_identifier) + Word(nums) + Optional(Suppress("%"))
+                Suppress(settings.quantity_identifier) 
+                + Word(nums)
+                + Optional(Suppress("%"))
                 ).set_results_name("quantity")
             order_type = one_of(
                 settings.order_type_identifier, caseless=True
                 ).set_results_name("order_type")
             leverage_type = one_of(
                 settings.leverage_type_identifier, caseless=True
                 ).set_results_name("leverage_type")
             comment = Combine(
-            Suppress(settings.comment_identifier) + Word(alphas)
+                    Suppress(settings.comment_identifier) 
+                    + Word(alphas)
                 ).set_results_name("comment")
 
-            #for action in settings.actions:
-            #print(f"{action.identifier} ({action.type})")
+            # for action in settings.actions:
+            # print(f"{action.identifier} ({action.type})")
             order_grammar = (
                 action("action")
-                + Optional(instrument,default=None)
-                + Optional(stop_loss,default=1000)
-                + Optional(take_profit,default=1000)
-                + Optional(quantity,default=1)
-                + Optional(order_type,default=None)
-                + Optional(leverage_type,default=None)
-                + Optional(comment,default=None)
+                + Optional(instrument, default=None)
+                + Optional(stop_loss, default=1000)
+                + Optional(take_profit, default=1000)
+                + Optional(quantity, default=1)
+                + Optional(order_type, default=None)
+                + Optional(leverage_type, default=None)
+                + Optional(comment, default=None)
               )
 
             order = order_grammar.parse_string(
                     instring=mystring,
                     parse_all=False
                     )
             logging.debug("identify_order %s", order)
@@ -100,14 +106,14 @@
             logging.debug("get_order %s", msg)
 
             if await self.search(msg):
                 logging.info("get_order found in %s", msg)
                 order = await self.identify_order(msg)
                 logging.info("order: %s", order)
                 if isinstance(order, dict):
-                    order["timestamp"] = datetime.datetime.now().strftime("%Y-%m-%dT%H:%M:%SZ")
+                    order["timestamp"] = datetime.now().strftime("%Y-%m-%dT%H:%M:%SZ")
                 return order
             return None
 
         except Exception as e:
             logging.exception("GetOrderError: %s", e)
             return None
```

### Comparing `findmyorder-1.2.4/pyproject.toml` & `findmyorder-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.2.4"
+version = "1.3.0"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
```

### Comparing `findmyorder-1.2.4/PKG-INFO` & `findmyorder-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.2.4
+Version: 1.3.0
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,14 @@
 
 
 | <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"> | A python package to identify and parse order for trade execution. |
 | ------------- | ------------- |
 |[![Pypi](https://badgen.net/badge/icon/findmyorder?icon=pypi&label)](https://pypi.org/project/findmyorder/) ![Version](https://img.shields.io/pypi/v/findmyorder)<br>  ![Pypi](https://img.shields.io/pypi/dm/findmyorder)<br> [![Build](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/findmyorder/branch/dev/graph/badge.svg?token=4838MSZNCC)](https://codecov.io/gh/mraniki/findmyorder) | Find & Parse a trade order for execution|
 
 
-
 Key features:
 
 - Identify an order with word `BUY SELL LONG SHORT` or your own `Bull`, `to the moon`, `pump` via config file
 - Parse and return a structured order with action and instrument as mandatory
 - Settings for custom option
```

