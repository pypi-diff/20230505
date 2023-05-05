# Comparing `tmp/sybil-scorer-0.0.0rc6.tar.gz` & `tmp/sybil-scorer-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sybil-scorer-0.0.0rc6.tar", last modified: Tue Jan 31 18:43:02 2023, max compression
+gzip compressed data, was "sybil-scorer-0.1.0rc1.tar", last modified: Fri May  5 19:45:13 2023, max compression
```

## Comparing `sybil-scorer-0.0.0rc6.tar` & `sybil-scorer-0.1.0rc1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-01-31 18:43:02.800941 sybil-scorer-0.0.0rc6/
--rw-rw-rw-   0        0        0     1084 2023-01-29 12:58:09.000000 sybil-scorer-0.0.0rc6/LICENSE
--rw-rw-rw-   0        0        0     9346 2023-01-31 18:43:02.800941 sybil-scorer-0.0.0rc6/PKG-INFO
--rw-rw-rw-   0        0        0     7407 2023-01-31 18:28:06.000000 sybil-scorer-0.0.0rc6/README.md
--rw-rw-rw-   0        0        0     1127 2023-01-31 18:17:40.000000 sybil-scorer-0.0.0rc6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-01-31 18:43:02.754066 sybil-scorer-0.0.0rc6/sbscorer/
-drwxrwxrwx   0        0        0        0 2023-01-31 18:43:02.768029 sybil-scorer-0.0.0rc6/sbscorer/sbdata/
--rw-rw-rw-   0        0        0    22791 2023-01-31 11:38:08.000000 sybil-scorer-0.0.0rc6/sbscorer/sbdata/FlipsideApi.py
--rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.0.0rc6/sbscorer/sbdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-31 18:43:02.772043 sybil-scorer-0.0.0rc6/sbscorer/sblegos/
--rw-rw-rw-   0        0        0    25475 2023-01-31 18:40:47.000000 sybil-scorer-0.0.0rc6/sbscorer/sblegos/TransactionAnalyser.py
--rw-rw-rw-   0        0        0        0 2023-01-21 08:46:58.000000 sybil-scorer-0.0.0rc6/sbscorer/sblegos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-31 18:43:02.776008 sybil-scorer-0.0.0rc6/sbscorer/sbutils/
--rw-rw-rw-   0        0        0     5318 2023-01-30 19:57:35.000000 sybil-scorer-0.0.0rc6/sbscorer/sbutils/LoadData.py
--rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.0.0rc6/sbscorer/sbutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-31 18:43:02.799942 sybil-scorer-0.0.0rc6/sbscorer/sybil_scorer.egg-info/
--rw-rw-rw-   0        0        0     9346 2023-01-31 18:43:02.000000 sybil-scorer-0.0.0rc6/sbscorer/sybil_scorer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2023-01-31 18:43:02.000000 sybil-scorer-0.0.0rc6/sbscorer/sybil_scorer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-31 18:43:02.000000 sybil-scorer-0.0.0rc6/sbscorer/sybil_scorer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2023-01-31 18:43:02.000000 sybil-scorer-0.0.0rc6/sbscorer/sybil_scorer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-01-31 18:43:02.000000 sybil-scorer-0.0.0rc6/sbscorer/sybil_scorer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      756 2023-01-31 18:43:02.806924 sybil-scorer-0.0.0rc6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 19:45:13.888712 sybil-scorer-0.1.0rc1/
+-rw-rw-rw-   0        0        0     1084 2023-01-29 12:58:09.000000 sybil-scorer-0.1.0rc1/LICENSE
+-rw-rw-rw-   0        0        0     9692 2023-05-05 19:45:13.889712 sybil-scorer-0.1.0rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     7755 2023-05-05 09:28:10.000000 sybil-scorer-0.1.0rc1/README.md
+-rw-rw-rw-   0        0        0     1125 2023-05-05 19:43:51.000000 sybil-scorer-0.1.0rc1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-05 19:45:13.811535 sybil-scorer-0.1.0rc1/sbscorer/
+drwxrwxrwx   0        0        0        0 2023-05-05 19:45:13.831405 sybil-scorer-0.1.0rc1/sbscorer/sbdata/
+-rw-rw-rw-   0        0        0    23088 2023-05-05 19:25:03.000000 sybil-scorer-0.1.0rc1/sbscorer/sbdata/FlipsideApi.py
+-rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.1.0rc1/sbscorer/sbdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:45:13.836444 sybil-scorer-0.1.0rc1/sbscorer/sblegos/
+-rw-rw-rw-   0        0        0    30403 2023-02-16 10:48:13.000000 sybil-scorer-0.1.0rc1/sbscorer/sblegos/TransactionAnalyser.py
+-rw-rw-rw-   0        0        0        0 2023-01-21 08:46:58.000000 sybil-scorer-0.1.0rc1/sbscorer/sblegos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:45:13.840757 sybil-scorer-0.1.0rc1/sbscorer/sbutils/
+-rw-rw-rw-   0        0        0     5318 2023-01-30 19:57:35.000000 sybil-scorer-0.1.0rc1/sbscorer/sbutils/LoadData.py
+-rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.1.0rc1/sbscorer/sbutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:45:13.887354 sybil-scorer-0.1.0rc1/sbscorer/sybil_scorer.egg-info/
+-rw-rw-rw-   0        0        0     9692 2023-05-05 19:45:13.000000 sybil-scorer-0.1.0rc1/sbscorer/sybil_scorer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-05-05 19:45:13.000000 sybil-scorer-0.1.0rc1/sbscorer/sybil_scorer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 19:45:13.000000 sybil-scorer-0.1.0rc1/sbscorer/sybil_scorer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-05-05 19:45:13.000000 sybil-scorer-0.1.0rc1/sbscorer/sybil_scorer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-05-05 19:45:13.000000 sybil-scorer-0.1.0rc1/sbscorer/sybil_scorer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      752 2023-05-05 19:45:13.891710 sybil-scorer-0.1.0rc1/setup.cfg
```

### Comparing `sybil-scorer-0.0.0rc6/LICENSE` & `sybil-scorer-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sybil-scorer-0.0.0rc6/PKG-INFO` & `sybil-scorer-0.1.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil-scorer
-Version: 0.0.0rc6
+Version: 0.1.0rc1
 Summary: A sybil scoring tool
 Home-page: https://github.com/poupou-web3/cluster-scorer
 Author: Poupou
 Author-email: Poupou <poupou-web3@protonmail.com>
 License: MIT License
         
         Copyright (c) 2023 Poupou
@@ -23,15 +23,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/poupou-web3/cluster-scorer
+Project-URL: Homepage, https://github.com/poupou-web3/sybil-scorer
 Project-URL: Documentation, https://sybil-scorer.readthedocs.io/en/latest/py-modindex.html
 Keywords: Sybil,OSS,Gitcoin,Quadratic
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -51,15 +51,15 @@
 
 The package has two main sub-packages.
 
 - **sbdata** is a package to easily retrieve a large amount of data from the flipside API.
 - **sblegos** a package to perform on-chain transactions analysis to detect potential Sybil behavior.
 - **sbutils** is a package that makes it easy to load the data extracted with sbdata and use it in sblegos.
 
-More details on the packages and example are provided below.
+More details on the packages and examples are provided below.
 
 ### sbdata
 
 An example script to retrieve data from the flipside API is provided in the script folder:
 script/demo_extract_eth_txs_oss.py
 
 It could also be used to retrieve transactional data from an address with some simple calls:
@@ -73,34 +73,34 @@
 address = ['0x06cd8288dc001024ce0a1cf39caaedc0e2db9c82']
 tx_add_eth = flipside_api.get_transactions(address, chain='ethereum')
 ```
 
 It walks you through the process of retrieving data from the flipside API and saving it in a folder.
 
 To use this package you will need an API key from flipside that you can get
-here : https://sdk.flipsidecrypto.xyz/shroomdk/apikeys
+here: https://sdk.flipsidecrypto.xyz/shroomdk/apikeys
 
 ### sblegos and sbutils
 
-sblegos provides the following analysis legos:
+sblegos provides the following analysis of legos:
 
 - **has_same_seed** : true if the address has the same seed as any other address in the grants contributors
 - **has_same_seed_naive** : true if the address has the same seed as any other address in the grants contributors with a
   naive approach: address of the from_address of the first transaction.
 - **has_suspicious_seed_behavior** : true if has_same_seed is different from has_same_seed_naive. It means the user
-  performed some actions before funding is wallet.
-- **has_interacted_with_other_contributor** : true if the user as interacted with any other contributor to the grant
+  performed some actions before funding his wallet.
+- **has_interacted_with_other_contributor** : true if the user has interacted with any other contributor to the grant
 - **has_less_than_n_transactions** : true if the user has less than n transactions.
 - **has_transaction_similitude** : true if the user has a transaction history that is similar to any other contributor
   to the grant.
 - **has_transaction_similitude_opti** : an optimized version of has_transaction_similitude, when used across multiple
   addresses.
 
 A jupyter notebook using both packages is available as a jupyter notebook
-here https://github.com/poupou-web3/grant-exploration/blob/main/gr-oss-exploration-application.ipynb
+here https://github.com/poupou-web3/grant-exploration/blob/main/gr-climate-exploration.ipynb
 
 The following snippet of code will check if any address has the same seed as any other contributor to the climate grant
 
 ``` python
 import os
 import sys
 from pathlib import Path
@@ -170,17 +170,18 @@
 The data provided by Gitcoin was standardized in the same format for all grants to make it easier to manipulate. For
 example to find all the wallet addresses of contributors to a specific project or grant.
 
 These can be recreated by using the files provided by ODC/Gitcoin. The files provided should be put with the
 architecture below. Each Grant is in a folder and inside there are the applications CSV and the votes CSV.
 
 Then run the jupyter notebook jupyter/normalize_contribution_data.ipynb
-this will create files in the root of the grant folder as shown below.
+this will create files in the root of the -explo
+folder as shown below.
 
-You can also download the standardized dara from Ocean market place here:
+You can also download the standardized data from Ocean market place here:
 
 - Standardized grant
   contributions : https://market.oceanprotocol.com/asset/did:op:eac43d546ba84e5b82ddf4d2fbf4db9290711e8d2c2a167bce148b7209d41623
 - standardized grant
   applications : https://market.oceanprotocol.com/asset/did:op:1d319077f7879e48b01aad52e4a69fc0ea06594c908575df4bd5cd015338b8cf
 
 ```commandline
@@ -218,7 +219,15 @@
 │       oss_grant_votes.csv
 │
 └───UNICEF
         unicef_grant_applications.csv
         unicef_grant_votes.csv
 ```
 
+## Future works
+
+Future works include:
+
+- Adding more transactional analysis lego.
+- Adding temporal features to a clustering algorithm as researched in the first
+  hackathon [submission](https://github.com/poupou-web3/GC-ODS-Sybil).
+- Adding legos using tags and labels of flipsidde API for example to filter similar seed wallet addresses.
```

### Comparing `sybil-scorer-0.0.0rc6/README.md` & `sybil-scorer-0.1.0rc1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 The package has two main sub-packages.
 
 - **sbdata** is a package to easily retrieve a large amount of data from the flipside API.
 - **sblegos** a package to perform on-chain transactions analysis to detect potential Sybil behavior.
 - **sbutils** is a package that makes it easy to load the data extracted with sbdata and use it in sblegos.
 
-More details on the packages and example are provided below.
+More details on the packages and examples are provided below.
 
 ### sbdata
 
 An example script to retrieve data from the flipside API is provided in the script folder:
 script/demo_extract_eth_txs_oss.py
 
 It could also be used to retrieve transactional data from an address with some simple calls:
@@ -33,34 +33,34 @@
 address = ['0x06cd8288dc001024ce0a1cf39caaedc0e2db9c82']
 tx_add_eth = flipside_api.get_transactions(address, chain='ethereum')
 ```
 
 It walks you through the process of retrieving data from the flipside API and saving it in a folder.
 
 To use this package you will need an API key from flipside that you can get
-here : https://sdk.flipsidecrypto.xyz/shroomdk/apikeys
+here: https://sdk.flipsidecrypto.xyz/shroomdk/apikeys
 
 ### sblegos and sbutils
 
-sblegos provides the following analysis legos:
+sblegos provides the following analysis of legos:
 
 - **has_same_seed** : true if the address has the same seed as any other address in the grants contributors
 - **has_same_seed_naive** : true if the address has the same seed as any other address in the grants contributors with a
   naive approach: address of the from_address of the first transaction.
 - **has_suspicious_seed_behavior** : true if has_same_seed is different from has_same_seed_naive. It means the user
-  performed some actions before funding is wallet.
-- **has_interacted_with_other_contributor** : true if the user as interacted with any other contributor to the grant
+  performed some actions before funding his wallet.
+- **has_interacted_with_other_contributor** : true if the user has interacted with any other contributor to the grant
 - **has_less_than_n_transactions** : true if the user has less than n transactions.
 - **has_transaction_similitude** : true if the user has a transaction history that is similar to any other contributor
   to the grant.
 - **has_transaction_similitude_opti** : an optimized version of has_transaction_similitude, when used across multiple
   addresses.
 
 A jupyter notebook using both packages is available as a jupyter notebook
-here https://github.com/poupou-web3/grant-exploration/blob/main/gr-oss-exploration-application.ipynb
+here https://github.com/poupou-web3/grant-exploration/blob/main/gr-climate-exploration.ipynb
 
 The following snippet of code will check if any address has the same seed as any other contributor to the climate grant
 
 ``` python
 import os
 import sys
 from pathlib import Path
@@ -130,17 +130,18 @@
 The data provided by Gitcoin was standardized in the same format for all grants to make it easier to manipulate. For
 example to find all the wallet addresses of contributors to a specific project or grant.
 
 These can be recreated by using the files provided by ODC/Gitcoin. The files provided should be put with the
 architecture below. Each Grant is in a folder and inside there are the applications CSV and the votes CSV.
 
 Then run the jupyter notebook jupyter/normalize_contribution_data.ipynb
-this will create files in the root of the grant folder as shown below.
+this will create files in the root of the -explo
+folder as shown below.
 
-You can also download the standardized dara from Ocean market place here:
+You can also download the standardized data from Ocean market place here:
 
 - Standardized grant
   contributions : https://market.oceanprotocol.com/asset/did:op:eac43d546ba84e5b82ddf4d2fbf4db9290711e8d2c2a167bce148b7209d41623
 - standardized grant
   applications : https://market.oceanprotocol.com/asset/did:op:1d319077f7879e48b01aad52e4a69fc0ea06594c908575df4bd5cd015338b8cf
 
 ```commandline
@@ -178,7 +179,15 @@
 │       oss_grant_votes.csv
 │
 └───UNICEF
         unicef_grant_applications.csv
         unicef_grant_votes.csv
 ```
 
+## Future works
+
+Future works include:
+
+- Adding more transactional analysis lego.
+- Adding temporal features to a clustering algorithm as researched in the first
+  hackathon [submission](https://github.com/poupou-web3/GC-ODS-Sybil).
+- Adding legos using tags and labels of flipsidde API for example to filter similar seed wallet addresses.
```

### Comparing `sybil-scorer-0.0.0rc6/pyproject.toml` & `sybil-scorer-0.1.0rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [build-system]
 requires = ['setuptools>=61.0.0', "wheel"]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "sybil-scorer"
-version = "0.0.0-rc6"
+version = "0.1.0-rc1"
 description = "A sybil scoring tool"
 readme = "README.md"
 authors = [{ name = "Poupou", email = "poupou-web3@protonmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["Sybil", "OSS", "Gitcoin", "Quadratic"]
 dependencies = [
-    "pandas==1.5.2",
-    "shroomdk==1.0.2",
+    "pandas==2.0.1",
+    "flipside==2.0.3",
     'tomli; python_version < "3.11"',
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["black",
     "jupyterlab==3.5.2",
     "ipykernel==6.20.2",
     "pip-tools",
     "pytest==7.2.1"]
 
 [project.urls]
-Homepage = "https://github.com/poupou-web3/cluster-scorer"
+Homepage = "https://github.com/poupou-web3/sybil-scorer"
 Documentation = "https://sybil-scorer.readthedocs.io/en/latest/py-modindex.html"
 
 [tool.setuptools.packages.find]
 where = ["sbscorer"]  # list of folders that contain the packages (["."] by default)
 include = ["sbdata", "sblegos", "sbutils"]
```

### Comparing `sybil-scorer-0.0.0rc6/sbscorer/sbdata/FlipsideApi.py` & `sybil-scorer-0.1.0rc1/sbscorer/sbdata/FlipsideApi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import os
 
 import numpy as np
 import pandas as pd
-from shroomdk import ShroomDK
+from flipside import Flipside
 
 
 def save_csv(df, path_to_export, csv_file):
     if not os.path.exists(path_to_export):
         os.makedirs(path_to_export)
     df.to_csv(csv_file, index=False)
 
 
 class FlipsideApi(object):
     """
     This class is used to query the flipside crypto api
     It has methods to easily retrieve the data and save it to csv
     """
 
-    def __init__(self, api_key, page_size=100000, timeout_minutes=4, page_number=1, max_address=100, ttl=60,
-                 cached=True, retry_interval=1):
+    def __init__(self, api_key, max_age_minutes=30, ttl=30, timeout_minutes=5, retry_interval=1, page_size=100000,
+                 page_number=1, max_address=100, cached=True):
         """
         Init method of FlipsideApi
         Parameters
         ----------
         api_key : str
             The api key to use to query flipside https://sdk.flipsidecrypto.xyz/shroomdk/apikeys
+        max_age_minutes : int
+            The max age in minutes of the query default is 30 because queries are also cached for 30 minutes
         page_size : int
             The number of rows to return per page default is 100000
         timeout_minutes : int
             The timeout in minutes default is 4
         page_number : int
             The page number to return default is 1
         max_address : int
@@ -38,16 +40,17 @@
         cached : bool
             If the query should be cached default is True. If you query several page it will run faster
         retry_interval : int
             The retry interval in seconds default is 1
         """
         self.api_key = api_key
 
-        # Initialize `ShroomDK`
-        self.sdk = ShroomDK(api_key)
+        # Initialize `FlipsideApi`
+        self.sdk = Flipside(api_key)
+        self.MAX_AGE_MINUTES = max_age_minutes
         # return up to 100,000 results per GET request on the query id
         self.PAGE_SIZE = page_size
         # timeout in minutes
         self.TIMEOUT_MINUTES = timeout_minutes
         # return results of page 1
         self.PAGE_NUMBER = page_number
         # max address to query.
@@ -113,14 +116,15 @@
         ----------
         Exception : Exception
             When the query times out. It will return an empty dataframe and then if you use the other methods will try
             to rerun with a smaller number of addresses.
         """
         try:
             query_result_set = self.sdk.query(sql,
+                                              max_age_minutes=self.MAX_AGE_MINUTES,
                                               page_size=self.PAGE_SIZE,
                                               page_number=page_number,
                                               timeout_minutes=self.TIMEOUT_MINUTES,
                                               ttl_minutes=self.TTL_MINUTES,
                                               cached=self.CACHED,
                                               retry_interval_seconds=self.RETRY_INTERVAL_SECONDS)
```

### Comparing `sybil-scorer-0.0.0rc6/sbscorer/sblegos/TransactionAnalyser.py` & `sybil-scorer-0.1.0rc1/sbscorer/sblegos/TransactionAnalyser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import sys
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
+import pylcs
 
 absolute_path = os.fspath(Path.cwd().parent.parent.parent)
 if absolute_path not in sys.path:
     sys.path.append(absolute_path)
 
 
 class TransactionAnalyser(object):
@@ -375,14 +376,93 @@
                 df_other_address.loc[add, 'lcs'] = 0
 
         df_similar_address = df_other_address.loc[df_other_address['lcs'] > 5, :]
         df_similar_address['score'] = df_similar_address.loc[:, 'lcs'].apply(
             lambda x: min(x / (len(array_transactions_target) / 2), 1))
         return df_similar_address
 
+    def transaction_similitude_pylcs(self, address, algo_type="address_only"):
+        """
+        Return a boolean and the list of addresses if it finds other addresses with similar actions.
+        it first store some repetitive tasks into a class attribute and then use it to speed up the process.
+
+        The algorithm is the following:
+        1. Transform all transactions in to a String of the form: "from_address,
+        to_address, from_address, to_address, ..."
+        2. Replace the address of the wallet by "x" to ba able to compare the behavior of two addresses.
+        3. Run the algorithm common longest substring on all the transactions
+        4. If the longest common substring is longer than 5, return true for the current address.
+        5. Keep iterating to find the longest common substring and then the score is
+        the length of the longest common substring divided by half the length of the target address string.
+        The score is the min(score, 1) to avoid having a score > 1.
+
+        Parameters
+        ----------
+        address : str
+            The address to check
+        algo_type : str
+            The type of algorithm to use. Default is "address_only" which only use the address to compare.
+            options are: address_only, address_and_value
+        char_tolerance : int
+            The number of character to skip when using the longest common substring algorithm. Default is 0.
+            1 may be a good choice when algo_type is "address_and_value".
+
+        Returns
+        -------
+        has_similar_behavior : bool
+            True if the address has similar behavior as another address
+        score_similar_behavior : float
+            The similarity score of the address
+        list_similar_address : map
+            The map of address and their similarity score
+
+        """
+
+        # Transform all transactions into a 1D string
+        if algo_type == "address_only" and self.dict_add_string_tx is None:
+            self.set_dict_add_string_transactions(algo_type)
+        elif algo_type == "address_and_value" and self.dict_add_value_string_tx is None:
+            self.set_dict_add_string_transactions(algo_type)
+        else:
+            Exception("algo_type not supported")
+
+        # Get all the transactions of the address in a 1D array
+        if algo_type == "address_only":
+            array_transactions_target = self.dict_add_string_tx.get(address)
+        elif algo_type == "address_and_value":
+            array_transactions_target = self.dict_add_value_string_tx.get(address)
+
+        shape_target = array_transactions_target.shape[0]
+        min_shape = max(1, shape_target / 4)
+        max_shape = max(shape_target, shape_target * 3)
+
+        # Get all the transactions from other contributors into an 1D array
+        df_other_address = self.df_address.loc[self.df_address['address'] != address, :]
+        df_other_address['lcs'] = 0
+        df_other_address.set_index('address', inplace=True)
+        for add in df_other_address.index:
+            df_other_address_transactions = self.get_address_transactions(add)
+            shape_other = df_other_address_transactions.shape[0]
+            if df_other_address_transactions.shape[0] <= 1:
+                df_other_address.loc[add, 'lcs'] = 0
+            elif min_shape < shape_other < max_shape:  # Heuristic to avoid comparing addresses with too different shapes
+                if algo_type == "address_only":
+                    array_transactions_other = self.dict_add_string_tx.get(add)
+                elif algo_type == "address_and_value":
+                    array_transactions_other = self.dict_add_value_string_tx.get(add)
+                lcs = self.longest_common_sub_string_pylcs(array_transactions_target, array_transactions_other)
+                df_other_address.loc[add, 'lcs'] = lcs
+            else:
+                df_other_address.loc[add, 'lcs'] = 0
+
+        df_similar_address = df_other_address.loc[df_other_address['lcs'] > 5, :]
+        df_similar_address['score'] = df_similar_address.loc[:, 'lcs'].apply(
+            lambda x: min(x / (len(array_transactions_target) / 2), 1))
+        return df_similar_address
+
     @staticmethod
     def get_array_transactions(df_address_transactions, address, algo_type="address_only"):
         """
         This method replace the target address by an arbitrary "x" to be able to compare the similitude of two wallet.
 
         Parameters
         ----------
@@ -402,22 +482,28 @@
         array_transactions : narray
             An array of strings
 
         """
         df_address_transactions.sort_values('block_timestamp', ascending=True, inplace=True)
         if algo_type == "address_only":
             try:
-                array_transactions = df_address_transactions.loc[:, ['from_address', 'to_address']].dropna().replace(
-                    address, 'x').agg('-'.join, axis=1).values
+                array_transactions = df_address_transactions.loc[:, ['from_address', 'to_address']].dropna() \
+                    .apply(lambda x: x.str[:8]) \
+                    .replace(address[:8], 'x') \
+                    .agg('-'.join, axis=1) \
+                    .values
             except Exception as e:
                 array_transactions = []
         elif algo_type == "address_and_value":
             try:
                 array_transactions = df_address_transactions.loc[:, ['from_address', 'value', 'to_address']].dropna() \
-                    .replace(address, 'x').agg('-'.join, axis=1).values
+                    .apply(lambda x: x.str[:8]) \
+                    .replace(address, 'x') \
+                    .agg('-'.join, axis=1) \
+                    .values
             except Exception as e:
                 array_transactions = []
         else:
             raise ValueError("algo_type must be either address_only or address_and_value")
         return array_transactions
 
     def has_transaction_similitude(self, address, algo_type="address_only", char_tolerance=0):
@@ -593,7 +679,16 @@
 
     def get_dict_string_tx(self, gb_address, algo_type="address_only"):
         dict_string_tx = {}
         for address, df_address in gb_address:
             array_transactions = self.get_array_transactions(df_address, address, algo_type)
             dict_string_tx[address] = array_transactions
         return dict_string_tx
+
+    @staticmethod
+    def longest_common_sub_string_pylcs(array_transactions_target, array_transactions_other):
+        string_target = "".join(array_transactions_target)
+        string_other = "".join(array_transactions_other)
+
+        # 1 similar transaction equals to 8 first char of the address + "-" + "x" = 10 char
+        lcs = pylcs.lcs_string_length(string_target, string_other)
+        return lcs // 10  # quotient of the division
```

### Comparing `sybil-scorer-0.0.0rc6/sbscorer/sbutils/LoadData.py` & `sybil-scorer-0.1.0rc1/sbscorer/sbutils/LoadData.py`

 * *Files identical despite different names*

### Comparing `sybil-scorer-0.0.0rc6/sbscorer/sybil_scorer.egg-info/PKG-INFO` & `sybil-scorer-0.1.0rc1/sbscorer/sybil_scorer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil-scorer
-Version: 0.0.0rc6
+Version: 0.1.0rc1
 Summary: A sybil scoring tool
 Home-page: https://github.com/poupou-web3/cluster-scorer
 Author: Poupou
 Author-email: Poupou <poupou-web3@protonmail.com>
 License: MIT License
         
         Copyright (c) 2023 Poupou
@@ -23,15 +23,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/poupou-web3/cluster-scorer
+Project-URL: Homepage, https://github.com/poupou-web3/sybil-scorer
 Project-URL: Documentation, https://sybil-scorer.readthedocs.io/en/latest/py-modindex.html
 Keywords: Sybil,OSS,Gitcoin,Quadratic
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -51,15 +51,15 @@
 
 The package has two main sub-packages.
 
 - **sbdata** is a package to easily retrieve a large amount of data from the flipside API.
 - **sblegos** a package to perform on-chain transactions analysis to detect potential Sybil behavior.
 - **sbutils** is a package that makes it easy to load the data extracted with sbdata and use it in sblegos.
 
-More details on the packages and example are provided below.
+More details on the packages and examples are provided below.
 
 ### sbdata
 
 An example script to retrieve data from the flipside API is provided in the script folder:
 script/demo_extract_eth_txs_oss.py
 
 It could also be used to retrieve transactional data from an address with some simple calls:
@@ -73,34 +73,34 @@
 address = ['0x06cd8288dc001024ce0a1cf39caaedc0e2db9c82']
 tx_add_eth = flipside_api.get_transactions(address, chain='ethereum')
 ```
 
 It walks you through the process of retrieving data from the flipside API and saving it in a folder.
 
 To use this package you will need an API key from flipside that you can get
-here : https://sdk.flipsidecrypto.xyz/shroomdk/apikeys
+here: https://sdk.flipsidecrypto.xyz/shroomdk/apikeys
 
 ### sblegos and sbutils
 
-sblegos provides the following analysis legos:
+sblegos provides the following analysis of legos:
 
 - **has_same_seed** : true if the address has the same seed as any other address in the grants contributors
 - **has_same_seed_naive** : true if the address has the same seed as any other address in the grants contributors with a
   naive approach: address of the from_address of the first transaction.
 - **has_suspicious_seed_behavior** : true if has_same_seed is different from has_same_seed_naive. It means the user
-  performed some actions before funding is wallet.
-- **has_interacted_with_other_contributor** : true if the user as interacted with any other contributor to the grant
+  performed some actions before funding his wallet.
+- **has_interacted_with_other_contributor** : true if the user has interacted with any other contributor to the grant
 - **has_less_than_n_transactions** : true if the user has less than n transactions.
 - **has_transaction_similitude** : true if the user has a transaction history that is similar to any other contributor
   to the grant.
 - **has_transaction_similitude_opti** : an optimized version of has_transaction_similitude, when used across multiple
   addresses.
 
 A jupyter notebook using both packages is available as a jupyter notebook
-here https://github.com/poupou-web3/grant-exploration/blob/main/gr-oss-exploration-application.ipynb
+here https://github.com/poupou-web3/grant-exploration/blob/main/gr-climate-exploration.ipynb
 
 The following snippet of code will check if any address has the same seed as any other contributor to the climate grant
 
 ``` python
 import os
 import sys
 from pathlib import Path
@@ -170,17 +170,18 @@
 The data provided by Gitcoin was standardized in the same format for all grants to make it easier to manipulate. For
 example to find all the wallet addresses of contributors to a specific project or grant.
 
 These can be recreated by using the files provided by ODC/Gitcoin. The files provided should be put with the
 architecture below. Each Grant is in a folder and inside there are the applications CSV and the votes CSV.
 
 Then run the jupyter notebook jupyter/normalize_contribution_data.ipynb
-this will create files in the root of the grant folder as shown below.
+this will create files in the root of the -explo
+folder as shown below.
 
-You can also download the standardized dara from Ocean market place here:
+You can also download the standardized data from Ocean market place here:
 
 - Standardized grant
   contributions : https://market.oceanprotocol.com/asset/did:op:eac43d546ba84e5b82ddf4d2fbf4db9290711e8d2c2a167bce148b7209d41623
 - standardized grant
   applications : https://market.oceanprotocol.com/asset/did:op:1d319077f7879e48b01aad52e4a69fc0ea06594c908575df4bd5cd015338b8cf
 
 ```commandline
@@ -218,7 +219,15 @@
 │       oss_grant_votes.csv
 │
 └───UNICEF
         unicef_grant_applications.csv
         unicef_grant_votes.csv
 ```
 
+## Future works
+
+Future works include:
+
+- Adding more transactional analysis lego.
+- Adding temporal features to a clustering algorithm as researched in the first
+  hackathon [submission](https://github.com/poupou-web3/GC-ODS-Sybil).
+- Adding legos using tags and labels of flipsidde API for example to filter similar seed wallet addresses.
```

### Comparing `sybil-scorer-0.0.0rc6/setup.cfg` & `sybil-scorer-0.1.0rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7962 696c 2d73 636f 7265 720d   = sybil-scorer.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e30  .version = 0.0.0
-00000030: 2d72 6336 0d0a 6175 7468 6f72 203d 2050  -rc6..author = P
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e30  .version = 0.1.0
+00000030: 2d72 6331 0d0a 6175 7468 6f72 203d 2050  -rc1..author = P
 00000040: 6f75 706f 750d 0a61 7574 686f 725f 656d  oupou..author_em
 00000050: 6169 6c20 3d20 706f 7570 6f75 2d77 6562  ail = poupou-web
 00000060: 3340 7072 6f74 6f6e 6d61 696c 2e63 6f6d  3@protonmail.com
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 4120 7379 6269 6c20 7363 6f72 696e 6720  A sybil scoring 
 00000090: 746f 6f6c 0d0a 6c6f 6e67 5f64 6573 6372  tool..long_descr
 000000a0: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
@@ -16,33 +16,32 @@
 000000f0: 646f 776e 0d0a 7572 6c20 3d20 6874 7470  down..url = http
 00000100: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
 00000110: 6f75 706f 752d 7765 6233 2f63 6c75 7374  oupou-web3/clust
 00000120: 6572 2d73 636f 7265 720d 0a70 726f 6a65  er-scorer..proje
 00000130: 6374 5f75 726c 7320 3d20 0d0a 0942 7567  ct_urls = ...Bug
 00000140: 2054 7261 636b 6572 203d 2068 7474 7073   Tracker = https
 00000150: 3a2f 2f67 6974 6875 622e 636f 6d2f 706f  ://github.com/po
-00000160: 7570 6f75 2d77 6562 332f 636c 7573 7465  upou-web3/cluste
-00000170: 722d 7363 6f72 6572 2f69 7373 7565 730d  r-scorer/issues.
-00000180: 0a09 7265 706f 7369 746f 7279 203d 2068  ..repository = h
-00000190: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000001a0: 6d2f 706f 7570 6f75 2d77 6562 332f 636c  m/poupou-web3/cl
-000001b0: 7573 7465 722d 7363 6f72 6572 0d0a 636c  uster-scorer..cl
-000001c0: 6173 7369 6669 6572 7320 3d20 0d0a 0950  assifiers = ...P
-000001d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000001e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000001f0: 2033 0d0a 094c 6963 656e 7365 203a 3a20   3...License :: 
-00000200: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-00000210: 4d49 5420 4c69 6365 6e73 650d 0a09 4f70  MIT License...Op
-00000220: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-00000230: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-00000240: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
-00000250: 6163 6b61 6765 5f64 6972 203d 200d 0a09  ackage_dir = ...
-00000260: 3d20 7362 7363 6f72 6572 0d0a 7061 636b  = sbscorer..pack
-00000270: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
-00000280: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-00000290: 3e3d 332e 3130 0d0a 0d0a 5b73 6264 6174  >=3.10....[sbdat
-000002a0: 612c 2073 626c 6567 6f73 2c20 7362 7574  a, sblegos, sbut
-000002b0: 696c 735d 0d0a 7768 6572 6520 3d20 7362  ils]..where = sb
-000002c0: 7363 6f72 6572 0d0a 0d0a 5b65 6767 5f69  scorer....[egg_i
-000002d0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-000002e0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-000002f0: 0d0a 0d0a                                ....
+00000160: 7570 6f75 2d77 6562 332f 7379 6269 6c2d  upou-web3/sybil-
+00000170: 7363 6f72 6572 2f69 7373 7565 730d 0a09  scorer/issues...
+00000180: 7265 706f 7369 746f 7279 203d 2068 7474  repository = htt
+00000190: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000001a0: 706f 7570 6f75 2d77 6562 332f 7379 6269  poupou-web3/sybi
+000001b0: 6c2d 7363 6f72 6572 0d0a 636c 6173 7369  l-scorer..classi
+000001c0: 6669 6572 7320 3d20 0d0a 0950 726f 6772  fiers = ...Progr
+000001d0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000001e0: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
+000001f0: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
+00000200: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+00000210: 4c69 6365 6e73 650d 0a09 4f70 6572 6174  License...Operat
+00000220: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+00000230: 2049 6e64 6570 656e 6465 6e74 0d0a 0d0a   Independent....
+00000240: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
+00000250: 6765 5f64 6972 203d 200d 0a09 3d20 7362  ge_dir = ...= sb
+00000260: 7363 6f72 6572 0d0a 7061 636b 6167 6573  scorer..packages
+00000270: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
+00000280: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
+00000290: 3130 0d0a 0d0a 5b73 6264 6174 612c 2073  10....[sbdata, s
+000002a0: 626c 6567 6f73 2c20 7362 7574 696c 735d  blegos, sbutils]
+000002b0: 0d0a 7768 6572 6520 3d20 7362 7363 6f72  ..where = sbscor
+000002c0: 6572 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  er....[egg_info]
+000002d0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+000002e0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

