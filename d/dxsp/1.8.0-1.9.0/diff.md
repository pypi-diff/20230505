# Comparing `tmp/dxsp-1.8.0.tar.gz` & `tmp/dxsp-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.8.0.tar", max compression
+gzip compressed data, was "dxsp-1.9.0.tar", max compression
```

## Comparing `dxsp-1.8.0.tar` & `dxsp-1.9.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-05-04 19:34:22.523761 dxsp-1.8.0/LICENSE
--rw-r--r--   0        0        0     3225 2023-05-04 19:34:22.523761 dxsp-1.8.0/README.md
--rw-r--r--   0        0        0       38 2023-05-04 19:34:22.523761 dxsp-1.8.0/dxsp/.gitignore
--rw-r--r--   0        0        0      169 2023-05-04 19:34:23.343767 dxsp-1.8.0/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-04 19:34:22.523761 dxsp-1.8.0/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-04 19:34:22.523761 dxsp-1.8.0/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      392 2023-05-04 19:34:22.523761 dxsp-1.8.0/dxsp/config.py
--rw-r--r--   0        0        0      556 2023-05-04 19:34:22.523761 dxsp-1.8.0/dxsp/default_settings.toml
--rw-r--r--   0        0        0    28404 2023-05-04 19:34:22.523761 dxsp-1.8.0/dxsp/main.py
--rw-r--r--   0        0        0     1787 2023-05-04 19:34:23.343767 dxsp-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     3979 1970-01-01 00:00:00.000000 dxsp-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-05 16:09:02.302583 dxsp-1.9.0/LICENSE
+-rw-r--r--   0        0        0     3215 2023-05-05 16:09:02.306584 dxsp-1.9.0/README.md
+-rw-r--r--   0        0        0       38 2023-05-05 16:09:02.306584 dxsp-1.9.0/dxsp/.gitignore
+-rw-r--r--   0        0        0      169 2023-05-05 16:09:03.298589 dxsp-1.9.0/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-05 16:09:02.306584 dxsp-1.9.0/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-05 16:09:02.306584 dxsp-1.9.0/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      392 2023-05-05 16:09:02.306584 dxsp-1.9.0/dxsp/config.py
+-rw-r--r--   0        0        0      556 2023-05-05 16:09:02.306584 dxsp-1.9.0/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    28403 2023-05-05 16:09:02.306584 dxsp-1.9.0/dxsp/main.py
+-rw-r--r--   0        0        0     1787 2023-05-05 16:09:03.298589 dxsp-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3969 1970-01-01 00:00:00.000000 dxsp-1.9.0/PKG-INFO
```

### Comparing `dxsp-1.8.0/LICENSE` & `dxsp-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.8.0/README.md` & `dxsp-1.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # DXSP (DeX SwaP)
 
 
 |<img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png">  | A python defi swap helper package. Swap made easy. |
 | ------------- | ------------- |
-|[![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br>[![🐍Build](https://github.com/mraniki/dxsp/actions/workflows/%F0%9F%90%8Dbuild.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%F0%9F%90%8Dbuild.yml) ![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|24 blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>2 swap protocol (1inch API, UniV2 router)
+|[![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br>[![✨Flow](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml) ![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|24 blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>2 swap protocol (1inch API, UniV2 router)
 
 
 
 Key features:
 
 - 24 blockchains mainnet and testnet supported with default block explorer, RPC, Router (uniswap and pancakeswap) and protocol url (1inch and 0x). Other blockchains can be supported via function attributes
 - 2 swap protocol type supported:
```

### Comparing `dxsp-1.8.0/dxsp/assets/blockchains.py` & `dxsp-1.9.0/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.8.0/dxsp/default_settings.toml` & `dxsp-1.9.0/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-1.8.0/dxsp/main.py` & `dxsp-1.9.0/dxsp/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                  dex_exchange: str | None = None,
                  dex_router: str | None = None,
                  amount_trading_option: int = 1,
                  ):
         """build a web3 object for swap"""
         self.logger = logging.getLogger(__name__)
         self.logger.info("DexSwap version: %s", __version__)
-        self.logger.info("Initializing DexSwap for %s on %s", 
+        self.logger.info("Initializing DexSwap for %s on %s",
                          wallet_address, chain_id)
 
         self.chain_id = int(chain_id)
         self.logger.debug("self.chain_id %s", self.chain_id)
         if self.chain_id is None:
             self.logger.warning("self.chain_id not setup")
             return
@@ -79,33 +79,33 @@
         self.protocol_type = protocol_type or "1inch"
         if self.protocol_type == "0x":
             base_url = blockchain["0x"]
         elif self.protocol_type == "1inch_limit":
             base_url = blockchain["1inch_limit"]
         else:
             base_url = blockchain["1inch"]
-        
+
         self.dex_url = f"{base_url}"
         self.logger.debug("self.dex_url %s", self.dex_url)
         self.logger.debug("self.protocol_type %s", self.protocol_type)
 
         self.dex_exchange = dex_exchange
         self.logger.debug("self.dex_exchange %s", self.dex_exchange)
 
         self.dex_router = dex_router
         if self.dex_router is None:
             if (
                 self.dex_exchange is None
                 or self.dex_exchange != blockchain["uniswap_v3"]
             ):
-                self.router = blockchain["uniswap_v2"]
+                self.router_contract_addr = blockchain["uniswap_v2"]
             else:
-                self.router = blockchain["uniswap_v3"]
+                self.router_contract_addr = blockchain["uniswap_v3"]
         else:
-            self.router = self.dex_router
+            self.router_contract_addr = self.dex_router
         self.logger.debug("self.router %s", self.router)
 
         self.name = "TBD"
         self.logger.debug("self.name %s", self.name)
 
         self.trading_quote_ccy = settings.trading_quote_ccy
         self.logger.debug("self.trading_quote_ccy %s", self.trading_quote_ccy)
@@ -115,279 +115,287 @@
 
         try:
             self.gecko_api = CoinGeckoAPI()
             assetplatform = self.gecko_api.get_asset_platforms()
             output_dict = [x for x in assetplatform if x['chain_identifier']
                            == int(self.chain_id)]
             self.gecko_platform = output_dict[0]['id']
-            self.logger.debug("self.gecko_platform %s",self.gecko_platform)
+            self.logger.debug("self.gecko_platform %s", self.gecko_platform)
         except Exception as e:
             self.logger.error("CoinGeckoAPI setup: %s", e)
             return
 
     async def _get(
                 self,
                 url,
                 params=None,
                 headers=None
             ):
         headers = {"User-Agent": "Mozilla/5.0"}
         self.logger.debug("_get url %s", url)
         response = requests.get(
                             url,
-                            params = params,
-                            headers = headers,
-                            timeout = 10
+                            params=params,
+                            headers=headers,
+                            timeout=10
                         )
         return response.json()
 
     async def get_quote(
                 self,
                 symbol
             ):
-        self.logger.debug("get_quote %s",symbol)
+        self.logger.debug("get_quote %s", symbol)
         asset_in_address = await self.search_contract(symbol)
         self.logger.debug("asset_in_address %s", asset_in_address)
         asset_out_symbol = self.trading_quote_ccy
         asset_out_address = await self.search_contract(asset_out_symbol)
-        self.logger.debug("asset_out_address %s",asset_out_address)
+        self.logger.debug("asset_out_address %s", asset_out_address)
         if asset_out_address is None:
-            self.logger.warning("No Valid Contract %s",symbol)
+            self.logger.warning("No Valid Contract %s", symbol)
             return
         # asset_out_contract = await self.get_token_contract(asset_out_symbol)
         # asset_out_decimals = asset_out_contract.functions.decimals().call()
         # self.logger.debug(f"asset_out_decimals {asset_out_decimals}")
         try:
             if self.protocol_type == "1inch":
-                asset_out_amount = self.w3.to_wei(1,'ether') #1USDC()
-                self.logger.debug("asset_out_amount %s",asset_out_amount)
+                asset_out_amount = self.w3.to_wei(1, 'ether')
+                self.logger.debug("asset_out_amount %s", asset_out_amount)
                 quote_url = f"{self.dex_url}/quote?fromTokenAddress={asset_in_address}&toTokenAddress={asset_out_address}&amount={asset_out_amount}"
                 quote = await self._get(quote_url)
-                self.logger.debug("quote %s",quote)
+                self.logger.debug("quote %s", quote)
                 raw_quote = quote['toTokenAmount']
-                self.logger.debug("raw_quote %s",raw_quote)
+                self.logger.debug("raw_quote %s", raw_quote)
                 asset_quote_decimals = quote['fromToken']['decimals']
                 self.logger.debug("asset_quote_decimals %s",
                                   asset_quote_decimals)
-                quote_readable = self.w3.from_wei(int(raw_quote),'wei') /(10 ** asset_quote_decimals)
-                self.logger.debug("quote_readable %s",quote_readable)
+                quote_readable = self.w3.from_wei(int(raw_quote), 'wei') / (10 ** asset_quote_decimals)
+                self.logger.debug("quote_readable %s", quote_readable)
                 return round(quote_readable, 2)
-            if self.protocol_type in ["uniswap_v2","uniswap_v3"]:
+            if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
                 return
         except Exception as e:
             self.logger.error("get_quote %s", e)
             return
 
-    async def execute_order(
-                self,
-                action,
-                instrument,
-                stop_loss=10000,
-                take_profit=10000,
-                quantity=1,
-                amount_trading_option=1,
-                order_type='swap'
-        ):
+    async def execute_order(self, order_params):
         """execute swap function"""
+        action = order_params.get('action')
+        instrument = order_params.get('instrument')
+        # stop_loss = order_params.get('stop_loss', 1000)
+        # take_profit = order_params.get('take_profit', 1000)
+        quantity = order_params.get('quantity', 1)
         try:
-            self.logger.debug("execute_order %s %s %s", action,instrument, order_type)
-            if order_type == 'swap':
-                self.logger.debug("execute_order %s",order_type)
-
-                asset_out_symbol = self.trading_quote_ccy if action == "BUY" else instrument
-                asset_in_symbol = instrument if action == "BUY" else self.trading_quote_ccy
-                asset_out_contract = await self.get_token_contract(asset_out_symbol)
-                try:
-                    asset_out_decimals = asset_out_contract.functions.decimals().call()
-                except Exception as e:
-                    self.logger.error("execute_order decimals: %s", e)
-                    asset_out_decimals = 18
-                asset_out_balance = await self.get_token_balance(asset_out_symbol)
-                if amount_trading_option == 1:
-                    # buy or sell %p percentage DEFAULT OPTION
-                    asset_out_amount = ((asset_out_balance)/
-                                        (10 ** asset_out_decimals))*(float(quantity)/100)
-                if amount_trading_option == 2:
-                    # SELL all token in case of sell order for example
-                    asset_out_amount = (asset_out_balance)/(10 ** asset_out_decimals)
-                order = await self.get_swap(
-                        asset_out_symbol,
-                        asset_in_symbol,
-                        asset_out_amount
-                        )
-                if order:
-                    return order['confirmation']
-
-            if order_type == "market":
-                self.logger.debug("execute_order %s", order_type)
-                return
-            if order_type == "limit":
-                self.logger.debug("execute_order %s", order_type)
-                return
+            asset_out_symbol = self.trading_quote_ccy if action == "BUY" else instrument
+            asset_in_symbol = instrument if action == "BUY" else self.trading_quote_ccy
+            asset_out_contract = await self.get_token_contract(asset_out_symbol)
+            try:
+                asset_out_decimals = asset_out_contract.functions.decimals().call()
+            except Exception as e:
+                self.logger.error("execute_order decimals: %s", e)
+                asset_out_decimals = 18
+            asset_out_balance = await self.get_token_balance(asset_out_symbol)
+            # if amount_trading_option == 2:
+            #     # SELL all token in case of sell order for example
+            #     asset_out_amount = (asset_out_balance)/(10 ** asset_out_decimals)
+            # else:
+            #     # buy or sell %p percentage DEFAULT OPTION
+            asset_out_amount = ((asset_out_balance)/
+                                (10 ** asset_out_decimals))*(float(quantity)/100)
+
+            order = await self.get_swap(
+                    asset_out_symbol,
+                    asset_in_symbol,
+                    asset_out_amount
+                    )
+            if order:
+                return order['confirmation']
 
         except Exception as e:
-            self.logger.debug("error execute_order %s",e)
+            self.logger.debug("error execute_order %s", e)
             return "error processing order in DXSP"
 
     async def get_swap(
                 self,
                 asset_out_symbol: str,
                 asset_in_symbol: str,
                 amount: int,
-                slippage_tolerance_percentage = 2
-        ):
+                slippage_tolerance_percentage=2
+                ):
         """main swap function"""
 
         self.logger.debug("get_swap %s %s %s", asset_out_symbol, asset_in_symbol, amount)
         try:
-            #ASSET OUT
+            # ASSET OUT
             asset_out_address = await self.search_contract(asset_out_symbol)
             asset_out_contract = await self.get_token_contract(asset_out_symbol)
-            self.logger.debug("asset_out_address %s %s",asset_out_address,asset_out_symbol)
+            self.logger.debug("asset_out_address %s %s", asset_out_address,asset_out_symbol)
             if asset_out_contract is None:
                 raise ValueError(f"Non contract identified for {asset_out_symbol}")
-            asset_out_decimals=asset_out_contract.functions.decimals().call()
+            asset_out_decimals = asset_out_contract.functions.decimals().call()
             asset_out_balance = await self.get_token_balance(asset_out_symbol)
             self.logger.debug("asset_out_balance %s",asset_out_balance)
             if asset_out_balance == 0:
                 self.logger.warning("No Money")
                 raise ValueError(f"Non contract identified for {asset_out_symbol}")
                 return
-            #ASSETS IN
+            # ASSETS IN
             asset_in_address = await self.search_contract(asset_in_symbol)
             self.logger.debug("asset_in_address %s", asset_in_address)
             if asset_in_address is None:
                 return
 
-            #AMOUNT
+            # AMOUNT
             asset_out_decimals = asset_out_contract.functions.decimals().call()
-            self.logger.debug("asset_out_decimals %s",asset_out_decimals)
+            self.logger.debug("asset_out_decimals %s", asset_out_decimals)
             asset_out_amount = amount * 10 ** asset_out_decimals
-            slippage = slippage_tolerance_percentage # defaulted to 2% slippage if not given
-            self.logger.debug("slippage %s",slippage)
+            # defaulted to 2% slippage if not given
+            slippage = slippage_tolerance_percentage  
+            self.logger.debug("slippage %s", slippage)
             asset_out_amount_converted = self.w3.to_wei(asset_out_amount,'ether')
 
-            transaction_amount = int((asset_out_amount_converted *(slippage/100)))
-            self.logger.debug("transaction_amount %s",transaction_amount)
+            order_amount = int((asset_out_amount_converted *(slippage/100)))
+            self.logger.debug("order_amount %s",order_amount)
 
-            #VERIFY IF ASSET OUT IS APPROVED otherwise get it approved
+            # VERIFY IF ASSET OUT IS APPROVED otherwise get it approved
             await self.get_approve(asset_out_address)
 
-            #1INCH
+            # 1INCH
             if self.protocol_type in ["1inch"]:
-                swap_url = f"{self.dex_url}/swap?fromTokenAddress={asset_out_address}&toTokenAddress={asset_in_address}&amount={transaction_amount}&fromAddress={self.wallet_address}&slippage={slippage}"
-                swap_TX = await self._get(swap_url)
-                TX_status_code = swap_TX['statusCode']
-                if TX_status_code != 200:
+                swap_url = f"{self.dex_url}/swap?fromTokenAddress={asset_out_address}&toTokenAddress={asset_in_address}&amount={order_amount}&fromAddress={self.wallet_address}&slippage={slippage}"
+                swap_order = await self._get(swap_url)
+                swap_order_status = swap_order['statusCode']
+                if swap_order_status != 200:
                     return
-            #UNISWAP V2
+            # UNISWAP V2
             if self.protocol_type in ["uniswap_v2"]:
-                order_path_dex=[asset_out_address, asset_in_address]
-                router_abi = await self.get_abi(self.router)
-                router_instance = self.w3.eth.contract(address=self.w3.to_checksum_address(self.router), abi=router_abi)
+                order_path_dex = [asset_out_address, asset_in_address]
+                router_abi = await self.get_abi(self.router_contract_addr)
+                router = self.w3.eth.contract(
+                                  self.w3.to_checksum_address(self.router_contract_addr),
+                                  router_abi)
                 deadline = self.w3.eth.get_block("latest")["timestamp"] + 3600
-                transaction_min_amount  = int(router_instance.functions.getAmountsOut(transaction_amount, order_path_dex).call()[1])
-                swap_TX = router_instance.functions.swapExactTokensForTokens(transaction_amount,transaction_min_amount,order_path_dex,self.wallet_address,deadline)
-            #1INCH LIMIT
+                order_min_amount = int(router.functions.getAmountsOut(
+                                        order_amount,
+                                        order_path_dex).call()[1])
+                swap_order = router.functions.swapExactTokensForTokens(
+                                                                                order_amount, 
+                                                                                order_min_amount,
+                                                                                order_path_dex,
+                                                                                self.wallet_address,
+                                                                                deadline)
+            # 1INCH LIMIT
             if self.protocol_type in ["1inch_limit"]:
-                 return
-                # encoded_message = encode_structured_data(eip712_data)
-                # signed_message = await sign_transaction_dex(encoded_message)
-                # # this is the limit order that will be broadcast to the limit order API
-                # limit_order = {
-                #     "orderHash": signed_message.messageHash.hex(),
-                #     "signature": signed_message.signature.hex(),
-                #     "data": order_data,
-                # }
-                # limit_order_url = dex_1inch_limit_api + str(chain_id) +"/limit-order" # make sure to change the chain_id if you are not using ETH mainnet
-                # response = requests.post(url=limit_order_url,headers={"accept": "application/json, text/plain, */*", "content-type": "application/json"}, json=limit_order)
+                return
 
-            #UNISWAP V3
+            # UNISWAP V3
             if self.protocol_type in ['uniswap_v3']:
                 return
-            if swap_TX:
-                self.logger.debug("swap_TX %s",swap_TX)
-                signed_TX = await self.get_sign(swap_TX)
-                transaction_hash = str(self.w3.to_hex(signed_TX))
-                #transaction_results = await self.get_block_explorer_status(transaction_hash)
-                transaction_hash_details = self.w3.wait_for_transaction_receipt(transaction_hash, timeout=120, poll_latency=0.1)
-                if transaction_hash_details['status'] == "1":
-                    transaction_blockNumber = transaction_hash_details['blockNumber']
-                    transaction_receipt = self.w3.eth.get_transaction_receipt(transaction_hash)
-                    transaction_block = self.w3.eth.get_block(transaction_blockNumber)
-                    order={}
-                    order['id'] = transaction_receipt['transactionHash']
-                    order['timestamp'] = transaction_block['timestamp']
-                    order['instrument'] = asset_out_symbol
-                    order['contract'] = asset_out_address
-                    order['amount'] = transaction_amount
-                    order['fee'] = transaction_receipt['gasUsed']
-                    order['price'] = "TBD"
-                    order['confirmation']= f"➕ Size: {order['amount']}\n\
-                                        ⚫️ Entry: {order['price']}\n\
-                                        ℹ️ {order['id']}\n\
-                                        🗓️ {order['timestamp']}"
-                    self.logger.info("order %s",order)
-                    return order
+            if swap_order:
+                self.logger.debug("swap_order %s", swap_order)
+                signed_order = await self.get_sign(swap_order)
+                order_hash = str(self.w3.to_hex(signed_order))
+                order_hash_details = self.w3.wait_for_transaction_receipt(
+                                            order_hash,
+                                            timeout=120,
+                                            poll_latency=0.1)
+                if order_hash_details['status'] == "1":
+                    await self.get_confirmation(
+                        order_hash,
+                        order_hash_details,
+                        asset_out_symbol,
+                        asset_out_address,
+                        order_amount,)
+        except Exception as e:
+            self.logger.error("get_swap %s", e)
+            return
+
+    async def get_confirmation(self,
+                               order_hash,
+                               order_hash_details,
+                               asset_out_symbol,
+                               asset_out_address,
+                               order_amount,
+                               ):
+        """ trade confirmation function"""
+        self.logger.debug("get_confirmation")
+        try:
+            order_blockNumber = order_hash_details['blockNumber']
+            order_receipt = self.w3.eth.get_transaction_receipt(order_hash)
+            order_block = self.w3.eth.get_block(order_blockNumber)
+            trade = {}
+            trade['id'] = order_receipt['transactionHash']
+            trade['timestamp'] = order_block['timestamp']
+            trade['instrument'] = asset_out_symbol
+            trade['contract'] = asset_out_address
+            trade['amount'] = order_amount
+            trade['fee'] = order_receipt['gasUsed']
+            trade['price'] = "TBD"
+            trade['confirmation'] = f"➕ Size: {trade['amount']}\n\
+                                ⚫️ Entry: {trade['price']}\n\
+                                ℹ️ {trade['id']}\n\
+                                🗓️ {trade['timestamp']}"
+            self.logger.info("trade %s", trade)
+            return trade
         except Exception as e:
-            self.logger.error("get_swap %s",e)
+            self.logger.error("get_confirmation %s", e)
             return
 
-    async def get_block_explorer_status(self,txHash):
-        self.logger.debug("get_block_explorer_status %s",txHash)
+    async def get_block_explorer_status(self, txHash):
+        self.logger.debug("get_block_explorer_status %s", txHash)
         checkTransactionSuccessURL = f"{self.block_explorer_url}?module=transaction&action=gettxreceiptstatus&txhash={txHash}&apikey={self.block_explorer_api}"
-        checkTransactionRequest =  self._get(checkTransactionSuccessURL)
+        checkTransactionRequest = self._get(checkTransactionSuccessURL)
         return checkTransactionRequest['status']
 
-####CONTRACT SEARCH
+# ###CONTRACT SEARCH
     async def search_contract(
-                            self, 
+                            self,
                             token
                             ):
         """search a contract function"""
         self.logger.debug("search_contract")
 
         try:
             token_contract = await self.get_contract_address(settings.TOKEN_PERSONAL_LIST,token)
             if token_contract is None:
                 token_contract = await self.get_contract_address(settings.TOKEN_TESTNET_LIST,token)
                 if token_contract is None:
                     token_contract = await self.get_contract_address(settings.TOKEN_MAINNET_LIST,token)
                     if token_contract is None:
                         token_contract = await self.search_gecko_contract(token)
             if token_contract is not None:
-                self.logger.info("token_contract found %s",token_contract)
+                self.logger.info("token_contract found %s", token_contract)
                 return self.w3.to_checksum_address(token_contract)
-            self.logger.info("no contract found for %s",token)
+            self.logger.info("no contract found for %s", token)
         except Exception as e:
-            self.logger.error("search_contract %s",e)
+            self.logger.error("search_contract %s", e)
             return
 
-    async def search_gecko(self,token):
+    async def search_gecko(self, token):
         """search coingecko"""
         self.logger.debug("search_gecko")
         try:
             search_results = self.gecko_api.search(query=token)
             search_dict = search_results['coins']
-            #self.logger.debug(f"search_dict {search_dict}")
-            filtered_dict = [x for x in search_dict if x['symbol'] == token.upper()]
-            api_dict = [ sub['api_symbol'] for sub in filtered_dict ]
-            self.logger.debug("api_dict %s",api_dict)
+            filtered_dict = [x for x in search_dict if
+                             x['symbol'] == token.upper()]
+            api_dict = [sub['api_symbol'] for sub in filtered_dict]
+            self.logger.debug("api_dict %s", api_dict)
             for i in api_dict:
                 coin_dict = self.gecko_api.get_coin_by_id(i)
                 try:
-                    if coin_dict['platforms'][f'{self.gecko_platform}'] is not None:
+                    if coin_dict['platforms'][f'{self.gecko_platform}']:
                         return coin_dict
                 except KeyError:
                     pass
         except Exception as e:
             self.logger.error("search_gecko %s", e)
             return
 
-    async def search_gecko_contract(self,token):
+    async def search_gecko_contract(self, token):
         """search coingecko contract"""
         self.logger.debug("🦎search_gecko_contract %s", token)
         self.logger.debug("🦎self.gecko_platform %s", self.gecko_platform)
         try:
             coin_info = await self.search_gecko(token)
             if coin_info is not None:
                 return coin_info['platforms'][f'{self.gecko_platform}']
@@ -396,158 +404,173 @@
             return
 
     async def get_contract_address(
                             self,
                             token_list_url,
                             symbol
                         ):
-        """Given a token symbol and json format url address tokenlist, get token address"""
-        self.logger.debug("get_contract_address %s %s",token_list_url, symbol)
+        """Given a token symbol and json format url address tokenlist, 
+        get token address"""
+        self.logger.debug("get_contract_address %s %s", token_list_url, symbol)
         try:
             token_list = await self._get(token_list_url)
             token_search = token_list['tokens']
             for keyval in token_search:
-                if (keyval['symbol'] == symbol and keyval['chainId'] == self.chain_id):
+                if (keyval['symbol'] == symbol and
+                    keyval['chainId'] == self.chain_id):
                     return keyval['address']
         except Exception as e:
             self.logger.debug("get_contract_address %s", e)
             return
 
     async def get_token_contract(
                                 self,
                                 token
                             ):
         """Given a token symbol, returns a contract object. """
-        self.logger.debug("get_token_contract %s",token)
+        self.logger.debug("get_token_contract %s", token)
         try:
             token_address = await self.search_contract(token)
             token_abi = await self.get_abi(token_address)
             return self.w3.eth.contract(address=token_address, abi=token_abi)
         except Exception as e:
-            self.logger.error("get_token_contract %s",e)
+            self.logger.error("get_token_contract %s", e)
             return
 
 
-####UTILS
+# ###UTILS
     async def get_approve(
                         self,
                         asset_out_address: str,
                         amount=None
                     ):
         self.logger.debug("get_approve %s", asset_out_address)
-        if self.protocol_type in ["1inch","1inch_limit"]:
+        if self.protocol_type in ["1inch", "1inch_limit"]:
             approval_check_URL = f"{self.dex_url}/approve/allowance?tokenAddress={asset_out_address}&walletAddress={self.wallet_address}"
             approval_response = await self._get(approval_check_URL)
             approval_check = approval_response['allowance']
-            if (approval_check==0):
+            if (approval_check == 0):
                 approval_URL = f"{self.dex_url}/approve/transaction?tokenAddress={asset_out_address}"
                 approval_response = await self._get(approval_URL)
-        elif self.protocol_type in ["uniswap_v2","uniswap_v3"]:
-            asset_out_abi= await self.get_abi(asset_out_address)
-            asset_out_contract = self.w3.eth.contract(address=asset_out_address, abi=asset_out_abi)
-            approval_check = asset_out_contract.functions.allowance(self.w3.to_checksum_address(self.wallet_address), self.w3.to_checksum_address(self.router)).call()
-            if (approval_check==0):
-                approved_amount = (self.w3.to_wei(2**64-1,'ether'))
+        elif self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
+            asset_out_abi = await self.get_abi(asset_out_address)
+            asset_out_contract = self.w3.eth.contract(
+                                 asset_out_address,
+                                 asset_out_abi)
+            approval_check = asset_out_contract.functions.allowance(
+                             self.w3.to_checksum_address(self.wallet_address),
+                             self.w3.to_checksum_address(self.router_contract_addr)
+                             ).call()
+            if (approval_check == 0):
+                approved_amount = (self.w3.to_wei(2**64-1, 'ether'))
                 asset_out_abi = await self.get_abi(asset_out_address)
-                asset_out_contract = self.w3.eth.contract(address=asset_out_address, abi=asset_out_abi)
-                approval_TX = asset_out_contract.functions.approve(self.w3.to_checksum_address(self.router), approved_amount)
+                asset_out_contract = self.w3.eth.contract(
+                                     asset_out_address,
+                                     asset_out_abi)
+                approval_TX = asset_out_contract.functions.approve(
+                                self.w3.to_checksum_address(self.router_contract_addr),
+                                approved_amount)
                 approval_txHash = await self.get_sign(approval_TX)
-                approval_txHash_complete = self.w3.eth.wait_for_transaction_receipt(approval_txHash, timeout=120, poll_latency=0.1)
+                approval_txHash_complete = self.w3.eth.wait_for_transaction_receipt(
+                                           approval_txHash,
+                                           timeout=120,
+                                           poll_latency=0.1)
 
     async def get_sign(
                     self,
-                    tx
+                    order
                 ):
-        self.logger.debug("get_sign %s", tx)
+        self.logger.debug("get_sign %s", order)
         try:
-            if not isinstance(tx, dict):
+            if not isinstance(order, dict):
                 raise ValueError("Transaction must be a dictionary")
-            if self.protocol_type in ['uniswap_v2','uniswap_v3']:
-                tx_params = {
-                'from': self.wallet_address,
-                'gas': await self.get_gas(tx),
-                'gasPrice': await self.get_gasPrice(tx),
-                'nonce': self.w3.eth.get_transaction_count(self.wallet_address),
-                }
-                tx = tx.build_transaction(tx_params)
+            if self.protocol_type in ['uniswap_v2', 'uniswap_v3']:
+                order_params = {
+                            'from': self.wallet_address,
+                            'gas': await self.get_gas(order),
+                            'gasPrice': await self.get_gasPrice(order),
+                            'nonce': self.w3.eth.get_transaction_count(
+                                self.wallet_address),
+                            }
+                order = order.build_transaction(order)
             elif self.protocol_type in ["1inch","1inch_limit"]:
-                tx = tx['tx']
-                tx['gas'] = await self.get_gas(tx)
-                tx['nonce'] = self.w3.eth.get_transaction_count(self.wallet_address)
-                tx['value'] = int(tx['value'])
-                tx['gasPrice'] = await self.get_gasPrice(tx)
-            signed = self.w3.eth.account.sign_transaction(tx, self.private_key)
-            raw_tx = signed.rawTransaction
-            return self.w3.eth.send_raw_transaction(raw_tx)
+                order = order['tx']
+                order['gas'] = await self.get_gas(order)
+                order['nonce'] = self.w3.eth.get_transaction_count(
+                    self.wallet_address)
+                order['value'] = int(order['value'])
+                order['gasPrice'] = await self.get_gasPrice(order)
+            signed = self.w3.eth.account.sign_transaction(
+                order,
+                self.private_key)
+            raw_order = signed.rawTransaction
+            return self.w3.eth.send_raw_transaction(raw_order)
         except (ValueError, TypeError, KeyError) as e:
             self.logger.error("get_sign: %s", e)
             raise
         except Exception as e:
             self.logger.error("get_sign: %s", e)
             raise RuntimeError("Failed to sign transaction")
 
     async def get_gas(
                     self,
                     tx
                 ):
         # Log the transaction
-        self.logger.debug("get_gas %s",tx)
+        self.logger.debug("get_gas %s", tx)
         # Estimate the gas cost of the transaction
-        gasestimate= self.w3.eth.estimate_gas(tx) * 1.25
+        gasestimate = self.w3.eth.estimate_gas(tx) * 1.25
         # Return the estimated gas cost in wei
-        return int(self.w3.to_wei(gasestimate,'wei'))
+        return int(self.w3.to_wei(gasestimate, 'wei'))
 
     async def get_gasPrice(self, tx):
         '''
         Get the gas price for a transaction
         '''
         self.logger.debug("get_gasPrice %s", tx)
         gasprice = self.w3.eth.generate_gas_price()
-        return self.w3.to_wei(gasprice,'gwei')
+        return self.w3.to_wei(gasprice, 'gwei')
 
-    async def get_abi(self,addr):
+    async def get_abi(self, addr):
         # Log a debug message to the logger
         self.logger.debug("get_abi %s", addr)
         if self.block_explorer_api:
             try:
                 # Create a dictionary of parameters
                 params = {
                     "module": "contract",
                     "action": "getabi",
                     "address": addr,
-                    "apikey": self.block_explorer_api }
+                    "apikey": self.block_explorer_api
+                    }
                 # Create a dictionary of headers
-                headers = { "User-Agent": "Mozilla/5.0" }
+                headers = {"User-Agent": "Mozilla/5.0"}
                 # Make a GET request to the block explorer URL
-                resp = await self._get(url=self.block_explorer_url,params=params,headers=headers)
+                resp = await self._get(
+                                       url = self.block_explorer_url,
+                                       params = params,
+                                       headers = headers
+                                       )
                 # If the response status is 1, log the ABI
                 if resp['status']=="1":
-                    self.logger.debug("ABI found %s",resp)
+                    self.logger.debug("ABI found %s", resp)
                     abi = resp["result"]
                     return abi
                 # If no ABI is identified, log a warning
                 self.logger.warning("No ABI identified for contract %s on chain %s",addr,self.chain_id)
             except Exception as e:
                 # Log an error
                 self.logger.error("error get_abi %s", e)
                 return
         else:
             # If no block_explorer_api is set, log a warning
             self.logger.warning("No block_explorer_api. Option B needed TBD")
-            return 
-
-
-#####USERS RELATED
+            return
 
-    # async def get_wallet_auth(self):
-    #     try:
-    #         return
-    #     except Exception as e:
-    #         self.logger.error("get_wallet_auth error: %s",e)
-    #         return
+# ####USERS RELATED
 
     async def get_token_balance(
                                 self,
                                 token
                             ):
         self.logger.debug("get_token_balance %s", token)
         try:
@@ -560,30 +583,28 @@
             token_contract = self.w3.eth.contract(address=token_address, abi=token_abi)
             token_balance = 0
             try:
                 token_balance = token_contract.functions.balanceOf(self.wallet_address).call()
             except ValueError as e:
                 self.logger.warning("Invalid address %s for token %s: %s", self.wallet_address, token, e)
             # (ex.from_wei(await fetch_token_balance(basesymbol), 'ether'), 5)
-            return 0 if token_balance <=0 else token_balance
+            return 0 if token_balance <= 0 else token_balance
         except Exception as e:
-            self.logger.error("get_token_balance %s: %s",token, e)
+            self.logger.error("get_token_balance %s: %s", token, e)
             return 0
 
-
     async def get_quote_ccy_balance(
                                 self
                             ):
         try:
             trading_quote_ccy_balance = await self.get_token_balance(self.trading_quote_ccy)
-                # return round(ex.from_wei(await fetch_token_balance(basesymbol), 'ether'), 5)
             return trading_quote_ccy_balance
-            # bal = round(ex.from_wei(bal,'ether'),5)
+
         except Exception as e:
-            self.logger.error("get_basecoin_balance %s: %s",token, e)
+            self.logger.error("get_basecoin_balance %s: %s", e)
             return 0
 
     async def get_stablecoin_balance(
                                 self
                             ):
         stablecoins = settings.stablecoins
         try:
@@ -604,20 +625,15 @@
             return self.w3.eth.get_balance(self.wallet_address)
         except Exception as e:
             self.logger.error("get_account_balance error: %s", e)
             return "balance error"
             # bal = round(ex.from_wei(bal,'ether'),5)
 
     async def get_account_position(
-                            self
-                        ):
+                                    self
+                                    ):
         try:
             self.logger.debug("get_account_position")
-            # asset_position_address= await search_contract(asset_out_symbol)
-            # asset_position_abi= await fetch_abi_dex(asset_out_address)
-            # asset_position_contract = ex.eth.contract(address=asset_out_address, abi=asset_out_abi)
-            # open_positions = asset_position_contract.functions.getOpenPositions(walletaddress).call()
             return
         except Exception as e:
             self.logger.error("get_account_position error: %s", e)
             return 0
-
```

### Comparing `dxsp-1.8.0/pyproject.toml` & `dxsp-1.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.8.0"
+version = "1.9.0"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-1.8.0/PKG-INFO` & `dxsp-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.8.0
+Version: 1.9.0
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 Description-Content-Type: text/markdown
 
 # DXSP (DeX SwaP)
 
 
 |<img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png">  | A python defi swap helper package. Swap made easy. |
 | ------------- | ------------- |
-|[![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br>[![🐍Build](https://github.com/mraniki/dxsp/actions/workflows/%F0%9F%90%8Dbuild.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%F0%9F%90%8Dbuild.yml) ![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|24 blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>2 swap protocol (1inch API, UniV2 router)
+|[![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br>[![✨Flow](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml) ![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|24 blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>2 swap protocol (1inch API, UniV2 router)
 
 
 
 Key features:
 
 - 24 blockchains mainnet and testnet supported with default block explorer, RPC, Router (uniswap and pancakeswap) and protocol url (1inch and 0x). Other blockchains can be supported via function attributes
 - 2 swap protocol type supported:
```

