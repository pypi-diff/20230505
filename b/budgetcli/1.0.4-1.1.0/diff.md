# Comparing `tmp/budgetcli-1.0.4.tar.gz` & `tmp/budgetcli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "budgetcli-1.0.4.tar", last modified: Sat Apr 29 18:41:58 2023, max compression
+gzip compressed data, was "budgetcli-1.1.0.tar", last modified: Fri May  5 21:50:23 2023, max compression
```

## Comparing `budgetcli-1.0.4.tar` & `budgetcli-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:41:58.841636 budgetcli-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-29 18:41:36.000000 budgetcli-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-29 18:41:58.841636 budgetcli-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-29 18:41:36.000000 budgetcli-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-29 18:41:36.000000 budgetcli-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-29 18:41:58.841636 budgetcli-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:41:58.837636 budgetcli-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:41:58.837636 budgetcli-1.0.4/src/budgetcli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:41:58.841636 budgetcli-1.0.4/src/budgetcli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/cli/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:41:58.841636 budgetcli-1.0.4/src/budgetcli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:41:58.841636 budgetcli-1.0.4/src/budgetcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-29 18:41:58.000000 budgetcli-1.0.4/src/budgetcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-29 18:41:58.000000 budgetcli-1.0.4/src/budgetcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:41:58.000000 budgetcli-1.0.4/src/budgetcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-29 18:41:58.000000 budgetcli-1.0.4/src/budgetcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-29 18:41:58.000000 budgetcli-1.0.4/src/budgetcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 18:41:58.000000 budgetcli-1.0.4/src/budgetcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:50:23.655035 budgetcli-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-05 21:49:55.000000 budgetcli-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-05 21:50:23.655035 budgetcli-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-05 21:49:55.000000 budgetcli-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-05 21:49:55.000000 budgetcli-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-05 21:50:23.655035 budgetcli-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:50:23.651034 budgetcli-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:50:23.655035 budgetcli-1.1.0/src/budgetcli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:50:23.655035 budgetcli-1.1.0/src/budgetcli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/cli/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:50:23.655035 budgetcli-1.1.0/src/budgetcli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:50:23.655035 budgetcli-1.1.0/src/budgetcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-05 21:50:23.000000 budgetcli-1.1.0/src/budgetcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-05 21:50:23.000000 budgetcli-1.1.0/src/budgetcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:50:23.000000 budgetcli-1.1.0/src/budgetcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 21:50:23.000000 budgetcli-1.1.0/src/budgetcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-05 21:50:23.000000 budgetcli-1.1.0/src/budgetcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 21:50:23.000000 budgetcli-1.1.0/src/budgetcli.egg-info/top_level.txt
```

### Comparing `budgetcli-1.0.4/LICENSE` & `budgetcli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.4/PKG-INFO` & `budgetcli-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,18 @@
-Metadata-Version: 2.1
-Name: budgetcli
-Version: 1.0.4
-Summary: A simple async budgeting app to manage expenses and budgets in google spreadsheets
-Author: Code Rustle
-Author-email: coderustle@gmail.com
-License: MIT
-Classifier: Topic :: Utilities
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Budget CLI
 
-[![Build](https://github.com/madalinpopa/budgetcli/actions/workflows/build.yaml/badge.svg)](https://github.com/madalinpopa/budgetcli/actions/workflows/build.yaml)
+[![Build](https://github.com/madalinpopa/budgetcli/actions/workflows/build.yaml/badge.svg)](https://github.com/madalinpopa/budgetcli/actions/workflows/build.yaml) [![Test](https://github.com/coderustle/budgetcli/actions/workflows/test.yaml/badge.svg)](https://github.com/coderustle/budgetcli/actions/workflows/test.yaml) [![License](https://img.shields.io/pypi/l/budgetcli)](https://img.shields.io/pypi/l/budgetcli)
 
 A simple terminal app written in Python to manage budgets and expenses in Google Sheet.
 
+## Features
+
+- Ability to track incomes and expenses as transactions
+- Ability to list transactions by month
+
 ## Installation
 
 ```
 pip install budgetcli
 ```
 
 In order to use the app you need first to enable Google Spreadsheet API and to generate app credentials with a
@@ -56,30 +46,50 @@
 
 ## Usage
 
 The commands follow the below structure.
 ```
 budgetcli <VERB> <OBJECT> <OPTIONS>
 ```
+### Incomes
+To add an income you need to provide only an amount and a category. By default, all the income transactions are added
+with default today date and without no description.
 
 **Add an income**
+```bash
+budgetcli add income 5000 Salary
+```
+**Add an income with description**
+```bash
+budgetcli add income 500 projects --description "Project A"
 ```
-budgetcli add income 2023-03-20 salary "short description" 4000
+**Add an income with date and description**
+```bash
+budgetcli add income 500 projects --description "Project A" --date 2023-04-01
 ```
+
+### Outcomes
+Same for outcome transactions, you need to provide only an amount and a category. By default, all the outcome transactions are added
+with default today date and without no description.
+
 **Add an outcome**
+```bash
+budgetcli add outcome 400 Rent
 ```
-budgetcli add outcome 2023-03-20 rent "short description" 400
+```bash
+budgetcli add outcome 400 Rent --date 2023-05-01 --description "Rent for April"
 ```
+### List transactions
 **List transactions. Default first 100 rows**
 ```
 budgetcli list transactions 
 ```
 **List only first 10 transactions**
 
-```
-budgetcli list transactions --rows=10 
+```bash
+budgetcli list transactions --rows 10 
 ```
 
 **List transactions for a specific month**
-```
-budgetcli list transactions --month=April 
+```bash
+budgetcli list transactions --month April 
 ```
```

### Comparing `budgetcli-1.0.4/setup.cfg` & `budgetcli-1.1.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = budgetcli
-version = 1.0.4
+version = 1.1.0
 author = Code Rustle
 author_email = coderustle@gmail.com
 description = A simple async budgeting app to manage expenses and budgets in google spreadsheets
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_file = LICENSE
```

### Comparing `budgetcli-1.0.4/src/budgetcli/auth.py` & `budgetcli-1.1.0/src/budgetcli/auth.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.4/src/budgetcli/cli/add.py` & `budgetcli-1.1.0/src/budgetcli/cli/add.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,76 @@
 """
-This module contains the commands for adding transactions to the google sheet
+This module contains the commands for adding transactions to the Google sheet
 """
+from datetime import date as date_obj
+from decimal import Decimal
 
 import typer
 
-from ..models import Transaction, validate_date, validate_amount
-from ..commands import AddTransactionCommand
+from ..commands import AddTransactionCommand, AddCategoryCommand
+from ..models import Transaction, Category, validate_amount, validate_date
+from ..utils.dates import get_today_date
 
 app = typer.Typer()
 
-DateArgument = typer.Argument(..., help="The date of the transaction")
+DateArgument = typer.Option(
+    get_today_date(), help="The date of the transaction"
+)
 CategoryArgument = typer.Argument(..., help="The category of the transaction")
-DescriptionArgument = typer.Argument(..., help="Transaction description")
+DescriptionArgument = typer.Option("", help="Transaction description")
 AmountArgument = typer.Argument(..., help="The amount of the transaction")
 
 
 @app.command()
+def category(name: str = CategoryArgument):
+    """Add a category to Google sheet"""
+    if name:
+        cat = Category(name)
+        command = AddCategoryCommand(cat)
+        command.execute()
+
+
+@app.command()
 def income(
-    date: str = DateArgument,
+    amount: str = AmountArgument,
     category: str = CategoryArgument,
     description: str = DescriptionArgument,
-    amount: str = AmountArgument,
+    date: str = DateArgument,
 ):
-    """Add an income transaction to the google sheet"""
-    transaction: Transaction | None = None
-
-    parsed_date = validate_date(date)
-    parsed_amount = validate_amount(amount)
+    """Add an income transaction to the Google sheet"""
+    parsed_date: date_obj | None = validate_date(date)
+    parsed_amount: Decimal | None = validate_amount(amount)
 
     if parsed_date and parsed_amount:
         transaction = Transaction(parsed_date, category, description)
         transaction.income = parsed_amount
-
-    if transaction:
         command = AddTransactionCommand(transaction)
         command.execute()
 
 
 @app.command()
 def outcome(
-    date: str = DateArgument,
+    amount: str = AmountArgument,
     category: str = CategoryArgument,
     description: str = DescriptionArgument,
-    amount: str = AmountArgument,
+    date: str = DateArgument,
 ):
-    """Add an outcome transaction to the google sheet"""
-    transaction: Transaction | None = None
-
-    parsed_date = validate_date(date)
-    parsed_amount = validate_amount(amount)
+    """Add an outcome transaction to the Google sheet"""
+    parsed_date: date_obj | None = validate_date(date)
+    parsed_amount: Decimal | None = validate_amount(amount)
 
     if parsed_date and parsed_amount:
         transaction = Transaction(parsed_date, category, description)
         transaction.outcome = parsed_amount
-
-    if transaction is not None:
         command = AddTransactionCommand(transaction)
         command.execute()
 
 
 @app.callback(invoke_without_command=True)
 def main(ctx: typer.Context):
-    """Add transactions to the google sheet"""
+    """Add transactions to the Google sheet"""
     if not ctx.invoked_subcommand:
         ctx.get_help()
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `budgetcli-1.0.4/src/budgetcli/cli/config.py` & `budgetcli-1.1.0/src/budgetcli/cli/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,17 @@
     to be copied in app config folder
     """
 
     if os.path.isfile(path):
         shutil.copy(path, CREDENTIALS_SECRET_PATH)
         update_config("client_secret", CREDENTIALS_SECRET_PATH)
 
-        print(f":heavy_check_mark: File copied succesfuly to {USER_CONFIG_DIR}")
+        print(
+            f":heavy_check_mark: File copied succesfuly to {USER_CONFIG_DIR}"
+        )
     else:
         print(f':x: The provided file path to "{path}" is not correct')
 
 
 @app.callback(invoke_without_command=True)
 def main(ctx: typer.Context) -> None:
     """Manage the configuration of the app"""
```

### Comparing `budgetcli-1.0.4/src/budgetcli/cli/display.py` & `budgetcli-1.1.0/src/budgetcli/cli/display.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import calendar
 import typer
 
 from ..utils.config import get_config_list
-from ..commands import ListTransactionCommand
+from ..commands import ListTransactionCommand, ListCategoryCommand
 from ..utils import dates
 
 app = typer.Typer()
 
 
 def validate_month(value: str | None) -> str | None:
     """A callback function to validate month input"""
@@ -32,14 +32,21 @@
     "",
     help="The name of the month eg: April or Apr",
     callback=validate_month,
 )
 
 
 @app.command()
+def categories(rows: int = RowsOption):
+    """List all categories from spreadsheet"""
+    command = ListCategoryCommand(rows=rows)
+    command.execute()
+
+
+@app.command()
 def transactions(rows: int = RowsOption, month: str = MonthOption):
     """List all transactions from spreadsheet"""
     month_number = dates.get_month_number(month)
     command = ListTransactionCommand(rows, month_number)
     command.execute()
```

### Comparing `budgetcli-1.0.4/src/budgetcli/data_manager.py` & `budgetcli-1.1.0/src/budgetcli/data_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,214 +1,308 @@
 import asyncio
 import json
-from typing import Any, TypeVar, Generic
-from abc import ABC
-from rich.pretty import pprint
+from abc import ABC, abstractmethod
+from typing import Coroutine, Generic, TypeVar
 
 import httpx
 from google.oauth2.credentials import Credentials
+from rich.pretty import pprint
 
 from .auth import load_user_token
 from .settings import API_URL, GVI_URL
 from .utils.config import get_config, update_config
 
 T = TypeVar("T", bound="AbstractDataManager")
 
 SPREADSHEET_ID = get_config("spreadsheet_id")
 
 
 class AbstractDataManager(ABC, Generic[T]):
+    """
+    Abstract class for data managers
+    """
+
+    PARAMS = [
+        "valueInputOption=USER_ENTERED",
+        "includeValuesInResponse=true",
+    ]
+
     def __init__(self):
         self.base_url = f"{API_URL}/{SPREADSHEET_ID}"
         self.gvi_url = f"{GVI_URL}/{SPREADSHEET_ID}/gviz/tq"
         self.session = httpx.AsyncClient()
         self.session.headers.update(self.get_auth_headers())
+        self.default_params = "?".join(self.PARAMS)
 
-    async def _append(
-        self, row: list[str], range: str
-    ) -> dict[str, str] | None:
+    @abstractmethod
+    async def init(self) -> None:
+        raise NotImplementedError
+
+    @abstractmethod
+    async def update(self, values: list[str], a1: str) -> dict[str, str]:
+        raise NotImplementedError
+
+    @abstractmethod
+    async def append(self, values: list[str]) -> dict[str, str]:
+        raise NotImplementedError
+
+    @abstractmethod
+    async def get_records(self, rows: int = 100):
+        raise NotImplementedError
+
+    async def _update(self, values: list[str], a1: str) -> dict[str, str]:
+        """Update a row or a specific cell"""
+        params = "valueInputOption=USER_ENTERED"
+        url = f"{self.base_url}/values/{a1}?{params}"
+        body = {"range": a1, "majorDimension": "ROWS", "values": [values]}
+        response = await self.session.put(url, json=body)
+        try:
+            response.raise_for_status()
+            data = response.json()
+            return data
+        except httpx.HTTPStatusError as err:
+            req_url = err.request.url
+            status = err.response.status_code
+            pprint(f"Error calling {req_url}, http status: {status}")
+        return {}
+
+    async def _append(self, values: list[str], a1: str) -> dict[str, str]:
         """Append row to sheet"""
         params = "valueInputOption=USER_ENTERED"
-        url = f"{self.base_url}/values/{range}:append?{params}"
-        body = {"majorDimension": "ROWS", "values": [row]}
+        url = f"{self.base_url}/values/{a1}:append?{params}"
+        body = {"majorDimension": "ROWS", "values": [values]}
         response = await self.session.post(url, json=body)
-
         try:
             response.raise_for_status()
+            data = response.json()
+            return data
         except httpx.HTTPStatusError as err:
             req_url = err.request.url
             status = err.response.status_code
             pprint(f"Error calling {req_url}, http status: {status}")
+        return {}
 
-    async def _list(self, range: str) -> dict[str, str] | None:
+    async def _list(self, a1: str) -> list[list[str]] | None:
         """List data from a given range"""
         params = "?majorDimension=ROWS"
-        url = f"{self.base_url}/values/{range}{params}"
+        url = f"{self.base_url}/values/{a1}{params}"
         response = await self.session.get(url)
         try:
             response.raise_for_status()
             result = response.json()
             return result.get("values", [])
         except httpx.HTTPStatusError as err:
             req_url = err.request.url
             status = err.response.status_code
             pprint(f"Error calling {req_url}, http status: {status}")
+        return None
 
-    async def _query(self, query: str, sheet_index: int) -> list[dict[str, list]] | None:
-        """A method to use Goolge Visualization API"""
+    async def _query(
+        self, query: str, sheet_index: int
+    ) -> list[dict[str, list]] | None:
+        """A method to use Google Visualization API"""
         params = f"gid={sheet_index}&tq={query}&tqx=out:json"
         url = f"{self.gvi_url}?{params}"
         response = await self.session.get(url)
         try:
             response.raise_for_status()
             to_replace = "/*O_o*/\ngoogle.visualization.Query.setResponse("
             clean_data = response.text.replace(to_replace, "")[:-2]
             json_data = json.loads(clean_data)
             rows = json_data.get("table", {}).get("rows", [])
             return rows
         except httpx.HTTPStatusError as err:
             req_url = err.request.url
             status = err.response.status_code
             pprint(f"Error calling {req_url}, http status: {status}")
+        return None
 
-    @staticmethod
-    def get_auth_headers() -> dict:
-        """Get the authentication headers from google credentials"""
-        headers = {}
-        credentials: Credentials | None = load_user_token()
-        if credentials:
-            credentials.apply(headers=headers)
-        return headers
-
-    async def sheet_exists(self, title: str) -> bool:
+    async def _get_sheet(self, title: str) -> dict[str, str] | None:
         """Check if the sheet with the given title exists"""
-        params = "fields=sheets.properties.title"
-        url = f"{self.base_url}?{params}"
-        response = await self.session.get(url)
-        try:
-            response.raise_for_status()
-            data = response.json()
-            sheets = data.get("sheets")
-            for sheet in sheets:
-                if sheet["properties"]["title"] == title:
-                    return True
-        except httpx.HTTPStatusError as err:
-            req_url = err.request.url
-            status = err.response.status_code
-            pprint(f"Error calling {req_url}, http status: {status}")
-        return False
-
-    async def get_sheet_index(self, title: str) -> int:
-        """Get google sheet index position"""
-        params = "fields=sheets"
+        params = "fields=sheets.properties"
         url = f"{self.base_url}?{params}"
         response = await self.session.get(url)
         try:
             response.raise_for_status()
             data = response.json()
             sheets = data.get("sheets")
             for sheet in sheets:
                 if sheet["properties"]["title"] == title:
-                    sheet_index = sheet["properties"]["index"]
-                    return sheet_index
+                    return sheet["properties"]
         except httpx.HTTPStatusError as err:
             req_url = err.request.url
             status = err.response.status_code
             pprint(f"Error calling {req_url}, http status: {status}")
-        return -1
+        return None
 
-    async def create_sheet(self, title: str) -> dict[str, str] | None:
-        """Create sheet with the given title"""
+    async def _create_sheet(self, title: str) -> dict[str, str] | None:
+        """Create sheet with the given title and returns its properties"""
         url = f"{self.base_url}/:batchUpdate"
         body = {"requests": [{"addSheet": {"properties": {"title": title}}}]}
         response = await self.session.post(url, json=body)
         try:
             response.raise_for_status()
             data = response.json()
-            replies = data.get('replies', []) 
+            replies = data.get("replies", [])
             sheet = replies[0].get("addSheet")
             properties = sheet.get("properties")
             return properties
         except httpx.HTTPStatusError as err:
             req_url = err.request.url
             status = err.response.status_code
             pprint(f"Error calling {req_url}, http status: {status}")
+        return None
+
+    async def _get_sheet_or_create(self, sheet_name: str) -> dict[str, str]:
+        """Get sheet or create if not exists"""
+        sheet: Coroutine = self._get_sheet(sheet_name)
+        try:
+            properties = await asyncio.wait_for(sheet, timeout=5)
+            if properties:
+                return properties
+            else:
+                create: Coroutine = self._create_sheet(sheet_name)
+                properties = await asyncio.wait_for(create, timeout=5)
+                if properties:
+                    return properties
+        except asyncio.TimeoutError:
+            pass
+        return {}
+
+    @staticmethod
+    def get_auth_headers() -> dict:
+        """Get the authentication headers from Google credentials"""
+        headers: dict[str, str] = {}
+        credentials: Credentials | None = load_user_token()
+        if credentials:
+            credentials.apply(headers=headers)
+        return headers
 
 
 class TransactionDataManager(AbstractDataManager):
-    SHEET_NAME = "TRANSACTIONS!"
+    SHEET_NAME = "TRANSACTIONS"
     FIRST_COLUMN = "A"
     LAST_COLUMN = "E"
-    TRANSACTIONS_RANGE = f"{SHEET_NAME}{FIRST_COLUMN}1:{LAST_COLUMN}"
+    ROW_START = 2
+    TRANSACTIONS_RANGE = (
+        f"{SHEET_NAME}!{FIRST_COLUMN}{ROW_START}:{LAST_COLUMN}"
+    )
+    HEADERS = ["DATE", "CATEGORY", "DESCRIPTION", "INCOME", "OUTCOME"]
 
-    async def init_sheet(self):
+    async def init(self) -> None:
         """Create TRANSACTIONS sheet if not exists"""
-        check = self.sheet_exists("TRANSACTIONS")
-        index = self.get_sheet_index("TRANSACTIONS")
+        a1 = f"{self.SHEET_NAME}!A1"
+        headers = "DATE CATEGORY DESCRIPTION INCOME OUTCOME"
+        sheet_coroutine: Coroutine = self._get_sheet_or_create(self.SHEET_NAME)
+        update_coroutine: Coroutine = self._update(headers.split(), a1)
         try:
-            exists = await asyncio.wait_for(check, timeout=5)
-            if exists:
-                index = await asyncio.wait_for(index, timeout=5)
+            sheet = await asyncio.wait_for(sheet_coroutine, timeout=5)
+            if sheet:
+                index = sheet["index"]
                 update_config("transactions_sheet_index", str(index))
-            else:
-                create = self.create_sheet("TRANSACTIONS")
-                properties = await asyncio.wait_for(create, timeout=5)
-                if properties:
-                    index =  properties.get("index")
-                    update_config("transactions_sheet_index", str(index))
+            await asyncio.wait_for(update_coroutine, timeout=5)
         except asyncio.TimeoutError:
             print("Timeout error")
 
-    async def get_transactions_for_month(
-        self, month: int 
-    ) -> list[list[str]] | None:
+    async def update(self, values: list[str], a1: str) -> dict[str, str]:
+        notation = f"{self.SHEET_NAME}!{a1}"
+        result = await self._update(values=values, a1=notation)
+        return result
+
+    async def append(self, values: list) -> dict[str, str]:
+        """Add a transaction to the spreadsheet"""
+        result = await self._append(values=values, a1=self.TRANSACTIONS_RANGE)
+        return result
+
+    async def get_records(self, rows: int = 100) -> list[list[str]]:
+        """List transactions. Default 100 rows"""
+        transaction_range = f"{self.TRANSACTIONS_RANGE}{rows + 1}"
+        result: list[list[str]] = await self._list(a1=transaction_range)
+        return result if result else []
+
+    async def get_records_for_month(self, month: int) -> list[list[str]]:
         """Query the transactions for current month"""
-        month = month - 1  # month query starts from 0 to 11
+        month -= 1  # month query starts from 0 to 11
         query = f"select A,B,C,D,E where month(A)={month}"
-        transactions = []
+
         sheet_index = get_config("transactions_sheet_index")
-        rows = None
-        if sheet_index:
-            index = int(sheet_index)
-            rows = await self._query(query, index)
-        else:
-            rows = await self._query(query, 0)
-        if rows:
-            for row in rows:
-                transaction = []
-                for cel in row.get("c", []):
-                    if "Date(" in str(cel.get("v")):
-                        date = cel.get("f")
-                        transaction.append(date)
-                    else:
-                        transaction.append(cel.get("v"))
-                transactions.append(transaction)
+        index = int(sheet_index) if sheet_index else 1
+        rows = await self._query(query, index)
+        transactions = [self._process_row(row) for row in rows] if rows else []
         return transactions
 
-    async def add_transaction(self, row: list) -> None:
-        """Add a transaction to the spreadsheet"""
-        await self._append(row=row, range=self.TRANSACTIONS_RANGE)
+    @staticmethod
+    def _process_row(row: dict[str, list]) -> list[str]:
+        """Helper function to process transaction rows"""
+        transaction = []
+        for cel in row.get("c", []):
+            if cel and "Date(" in str(cel.get("v")):
+                date = cel.get("f")
+                transaction.append(date)
+            elif cel:
+                transaction.append(cel.get("v"))
+            else:
+                transaction.append("")
+        return transaction
 
-    async def list_transactions(self, rows: int = 100) -> list[list[str]]:
-        """List transactions. Default 100 rows"""
-        transaction_range = f"{self.TRANSACTIONS_RANGE}{rows}"
-        result = await self._list(range=transaction_range)
-        if result:
-            check_rows = all(isinstance(row, list) for row in result)
-            check_columns = all(
-                isinstance(col, str) for rows in result for col in rows
-            )
-            if isinstance(result, list) and check_rows and check_columns:
-                return result
-        return []
+
+class CategoryDataManager(AbstractDataManager):
+    SHEET_NAME = "CATEGORIES"
+    FIRST_COLUMN = "A"
+    LAST_COLUMN = "A"
+    ROW_START = 2
+    CATEGORY_RANGE = f"{SHEET_NAME}!{FIRST_COLUMN}{ROW_START}:{LAST_COLUMN}"
+
+    async def init(self) -> None:
+        """Create CATEGORY sheet if not exists"""
+        a1 = f"{self.SHEET_NAME}!A1"
+        headers = "CATEGORY"
+        sheet_coroutine: Coroutine = self._get_sheet_or_create(self.SHEET_NAME)
+        update_coroutine: Coroutine = self._update([headers], a1)
+        try:
+            sheet = await asyncio.wait_for(sheet_coroutine, timeout=5)
+            if sheet:
+                index = sheet["index"]
+                update_config("categories_sheet_index", str(index))
+            await asyncio.wait_for(update_coroutine, timeout=5)
+        except asyncio.TimeoutError:
+            print("Timeout error")
+
+    async def update(self, values: list[str], a1: str) -> dict[str, str]:
+        notation = f"{self.SHEET_NAME}!{a1}"
+        result = await self._update(values=values, a1=notation)
+        return result
+
+    async def append(self, values: list) -> dict[str, str]:
+        """Add new category in Google sheet"""
+        result = await self._append(values=values, a1=self.CATEGORY_RANGE)
+        return result
+
+    async def get_records(self, rows: int = 100):
+        """Return all categories"""
+        category_range = f"{self.CATEGORY_RANGE}{rows + 1}"
+        result: list[list[str]] = await self._list(a1=category_range)
+        return result if result else []
+
+    async def get_records_by_name(self, name: str) -> None:
+        """Return a category by a given name"""
+        name = name.lower()
+        query = f"select A where A='{name}'"
+        index = get_config("categories_sheet_index")
+        print("index is", index)
+        if index:
+            rows = await self._query(query, int(index))
+            pprint(rows, expand_all=True)
+            return rows
 
 
 class ManagerFactory:
     @staticmethod
-    def create_manager_for(manager_name: str) -> Any | None:
+    def create_manager_for(manager_name: str) -> T | None:
         match manager_name:
             case "transactions":
                 return TransactionDataManager()
             case "categories":
-                pass
+                return CategoryDataManager()
             case _:
                 pprint("No manager found")
+        return None
```

### Comparing `budgetcli-1.0.4/src/budgetcli/main.py` & `budgetcli-1.1.0/src/budgetcli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import asyncio
 import typer
 from rich import print
 
 from .auth import get_user_authorization
 from .cli import add, config, display
-from .commands import InitTransactionCommand
+from .commands import InitCommand
 
 # init typer app
 app = typer.Typer()
 
 # register commands
 app.add_typer(config.app, name="config")
 app.add_typer(add.app, name="add")
@@ -16,24 +15,24 @@
 
 
 @app.command()
 def auth():
     """Authorize the app to use the user data"""
     try:
         get_user_authorization()
-        print(":heavy_check_mark: User authorized succesfuly")
+        print(":heavy_check_mark: User authorized successfully")
     except Exception as e:
         print(":x: Error authorizing user")
         print(e)
 
 
 @app.command()
 def init():
-    """Init the sheets in the google spreadsheets"""
-    command = InitTransactionCommand()
+    """Init the sheets in the Google spreadsheets"""
+    command = InitCommand()
     command.execute()
 
 
 @app.callback(invoke_without_command=True)
 def main(ctx: typer.Context) -> None:
     if ctx.invoked_subcommand is None:
         ctx.get_help()
```

### Comparing `budgetcli-1.0.4/src/budgetcli/settings.py` & `budgetcli-1.1.0/src/budgetcli/settings.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.4/src/budgetcli/utils/config.py` & `budgetcli-1.1.0/src/budgetcli/utils/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ..settings import CONFIG_FILE_PATH
 
 
 def get_config_list():
     """Utility function to list all the settings from config.json"""
 
     if os.path.exists(CONFIG_FILE_PATH):
-        config: dict
+        config: dict[str, str]
 
         with open(CONFIG_FILE_PATH) as file:
             config = json.load(file)
 
         pprint(config, expand_all=True)
 
     else:
@@ -23,34 +23,29 @@
 
 
 def update_config(setting: str, value: str) -> None:
     """Utility function to update config.json file"""
 
     if os.path.exists(CONFIG_FILE_PATH):
         config: dict
-
         with open(CONFIG_FILE_PATH) as file:
             config = json.load(file)
             config[setting] = value
-
         with open(CONFIG_FILE_PATH, "w") as file:
             json.dump(config, file, indent=2)
-
     else:
         config = {setting: value}
-
         with open(CONFIG_FILE_PATH, "w") as file:
             json.dump(config, file, indent=2)
-
     print(f":heavy_check_mark: {setting} was updated")
 
 
 def get_config(setting: str) -> str | None:
     """Utility function to retrieve a setting from config.json"""
 
     if os.path.exists(CONFIG_FILE_PATH):
         config: dict
 
         with open(CONFIG_FILE_PATH) as file:
             config = json.load(file)
-
         return config.get(setting)
+    return None
```

### Comparing `budgetcli-1.0.4/src/budgetcli/utils/dates.py` & `budgetcli-1.1.0/src/budgetcli/utils/dates.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 
 def get_current_month():
     """An utility function to return the current month number"""
     now = datetime.now()
     return now.month
 
 
+def get_today_date():
+    """An utility function to return today's date"""
+    now = datetime.now()
+    return now.strftime("%d-%m-%Y")
+
+
 def get_month_number(month: str) -> int | None:
     """An utility function to return the month number from the month name"""
     month_str = month.lower()
     for i, month in enumerate(calendar.month_name[1:], 1):
         abbr = calendar.month_abbr[i].lower()
         if month_str == month.lower() or month_str == abbr:
             return i
+    return None
```

### Comparing `budgetcli-1.0.4/src/budgetcli/utils/display.py` & `budgetcli-1.1.0/src/budgetcli/utils/display.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from rich import box, print
 from rich.table import Table
 from rich.progress import Progress, SpinnerColumn, TextColumn
 
 
 @contextmanager
 def task_progress(description: str):
-    """An utility function to display a progress spinner"""
+    """A utility function to display a progress spinner"""
     start_time = time.time()
     spinner = SpinnerColumn()
     text = TextColumn("[progress.description]{task.description}")
     try:
         with Progress(spinner, text, transient=True) as progress:
             progress.add_task(description=description, total=None)
             yield
@@ -21,13 +21,20 @@
         elapsed_time = end_time - start_time
         print(f":sparkles: Completed in {elapsed_time:.2f} seconds")
 
 
 def get_transaction_table() -> Table:
     """Return table to display the transaction date"""
     table = Table(header_style="blue", box=box.HORIZONTALS)
-    table.add_column("Date", justify="left", no_wrap=True)
-    table.add_column("Category", justify="left", no_wrap=True)
-    table.add_column("Description", justify="left", no_wrap=True)
-    table.add_column("Income", justify="left", no_wrap=True, style="green")
-    table.add_column("Outcome", justify="left", no_wrap=True, style="red")
+    table.add_column("Date", no_wrap=True)
+    table.add_column("Category", no_wrap=True)
+    table.add_column("Description", no_wrap=True)
+    table.add_column("Income", no_wrap=True, style="green")
+    table.add_column("Outcome", no_wrap=True, style="red")
+    return table
+
+
+def get_category_table() -> Table:
+    """Return table to display categories"""
+    table = Table(header_style="blue", box=box.HORIZONTALS)
+    table.add_column("Category", no_wrap=True)
     return table
```

### Comparing `budgetcli-1.0.4/src/budgetcli.egg-info/PKG-INFO` & `budgetcli-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: budgetcli
-Version: 1.0.4
+Version: 1.1.0
 Summary: A simple async budgeting app to manage expenses and budgets in google spreadsheets
 Author: Code Rustle
 Author-email: coderustle@gmail.com
 License: MIT
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Budget CLI
 
-[![Build](https://github.com/madalinpopa/budgetcli/actions/workflows/build.yaml/badge.svg)](https://github.com/madalinpopa/budgetcli/actions/workflows/build.yaml)
+[![Build](https://github.com/madalinpopa/budgetcli/actions/workflows/build.yaml/badge.svg)](https://github.com/madalinpopa/budgetcli/actions/workflows/build.yaml) [![Test](https://github.com/coderustle/budgetcli/actions/workflows/test.yaml/badge.svg)](https://github.com/coderustle/budgetcli/actions/workflows/test.yaml) [![License](https://img.shields.io/pypi/l/budgetcli)](https://img.shields.io/pypi/l/budgetcli)
 
 A simple terminal app written in Python to manage budgets and expenses in Google Sheet.
 
+## Features
+
+- Ability to track incomes and expenses as transactions
+- Ability to list transactions by month
+
 ## Installation
 
 ```
 pip install budgetcli
 ```
 
 In order to use the app you need first to enable Google Spreadsheet API and to generate app credentials with a
@@ -56,30 +61,50 @@
 
 ## Usage
 
 The commands follow the below structure.
 ```
 budgetcli <VERB> <OBJECT> <OPTIONS>
 ```
+### Incomes
+To add an income you need to provide only an amount and a category. By default, all the income transactions are added
+with default today date and without no description.
 
 **Add an income**
+```bash
+budgetcli add income 5000 Salary
 ```
-budgetcli add income 2023-03-20 salary "short description" 4000
+**Add an income with description**
+```bash
+budgetcli add income 500 projects --description "Project A"
 ```
+**Add an income with date and description**
+```bash
+budgetcli add income 500 projects --description "Project A" --date 2023-04-01
+```
+
+### Outcomes
+Same for outcome transactions, you need to provide only an amount and a category. By default, all the outcome transactions are added
+with default today date and without no description.
+
 **Add an outcome**
+```bash
+budgetcli add outcome 400 Rent
 ```
-budgetcli add outcome 2023-03-20 rent "short description" 400
+```bash
+budgetcli add outcome 400 Rent --date 2023-05-01 --description "Rent for April"
 ```
+### List transactions
 **List transactions. Default first 100 rows**
 ```
 budgetcli list transactions 
 ```
 **List only first 10 transactions**
 
-```
-budgetcli list transactions --rows=10 
+```bash
+budgetcli list transactions --rows 10 
 ```
 
 **List transactions for a specific month**
-```
-budgetcli list transactions --month=April 
+```bash
+budgetcli list transactions --month April 
 ```
```

### Comparing `budgetcli-1.0.4/src/budgetcli.egg-info/SOURCES.txt` & `budgetcli-1.1.0/src/budgetcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

