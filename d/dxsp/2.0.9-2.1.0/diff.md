# Comparing `tmp/dxsp-2.0.9.tar.gz` & `tmp/dxsp-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.0.9.tar", max compression
+gzip compressed data, was "dxsp-2.1.0.tar", max compression
```

## Comparing `dxsp-2.0.9.tar` & `dxsp-2.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-08 13:45:01.323274 dxsp-2.0.9/LICENSE
--rw-r--r--   0        0        0     3349 2023-05-08 13:45:01.323274 dxsp-2.0.9/README.md
--rw-r--r--   0        0        0       86 2023-05-08 13:45:02.315296 dxsp-2.0.9/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-08 13:45:01.323274 dxsp-2.0.9/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-08 13:45:01.323274 dxsp-2.0.9/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-08 13:45:01.323274 dxsp-2.0.9/dxsp/config.py
--rw-r--r--   0        0        0     3109 2023-05-08 13:45:01.323274 dxsp-2.0.9/dxsp/default_settings.toml
--rw-r--r--   0        0        0    25292 2023-05-08 13:45:01.323274 dxsp-2.0.9/dxsp/main.py
--rw-r--r--   0        0        0     1790 2023-05-08 13:45:02.315296 dxsp-2.0.9/pyproject.toml
--rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 dxsp-2.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-09 19:27:31.057859 dxsp-2.1.0/LICENSE
+-rw-r--r--   0        0        0     2595 2023-05-09 19:27:31.057859 dxsp-2.1.0/README.md
+-rw-r--r--   0        0        0       86 2023-05-09 19:27:31.733866 dxsp-2.1.0/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-09 19:27:31.057859 dxsp-2.1.0/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-09 19:27:31.057859 dxsp-2.1.0/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-09 19:27:31.057859 dxsp-2.1.0/dxsp/config.py
+-rw-r--r--   0        0        0     3386 2023-05-09 19:27:31.057859 dxsp-2.1.0/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    26120 2023-05-09 19:27:31.057859 dxsp-2.1.0/dxsp/main.py
+-rw-r--r--   0        0        0     1790 2023-05-09 19:27:31.733866 dxsp-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3328 1970-01-01 00:00:00.000000 dxsp-2.1.0/PKG-INFO
```

### Comparing `dxsp-2.0.9/LICENSE` & `dxsp-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.9/README.md` & `dxsp-2.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,49 +5,39 @@
 | ------------- | ------------- |
 |[![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br>[![✨Flow](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH)](https://codecov.io/gh/mraniki/dxsp) <br>![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|24 blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>2 swap protocol (1inch API, UniV2 router)
 
 
 
 Key features:
 
-- 24 blockchains mainnet and testnet supported with default block explorer, RPC, Router (uniswap and pancakeswap) and protocol url (1inch and 0x). Other blockchains can be supported via function attributes
+- Any blockchains mainnet or testnet supported by web3py, 1inch or uniswap type router.
 - 2 swap protocol type supported:
 	- 1inch API v5
 	- Uniswap version 2 router protocol type
 
 Other features:
 - Translate token symbol to contract address via user defined tokenlist format or coingecko api 
-- Connect to web3  if no web3 object or no rpc provided
+- Connect to web3 if no web3 object or no rpc provided
 - Able to approve contract and sign transaction
 - Quote for a given token
 - Use Base symbol like stablecoin
-
+- Settings to use the modile for your own tool/bot
 
 
 # Install
 `pip install dxsp`
 
 # How to use it
 ```
 from dxsp import DexSwap
 
-	#SWAP HELPER
-	dex = DexSwap(chain_id=chain_id,wallet_address=wallet_address,private_key=private_key,block_explorer_api=block_explorer_api)
-	print("dex ", dex)
+	dex = DexSwap()
 	#BUY 10 USDC to SWAP with BITCOIN
 	demo_tx = await dex.get_swap('USDT','wBTC',10)
 	print("demo_tx ", demo_tx)
-
-	#SWAP with your OWN defined exchange like Sushiswap on ARBITRUM 
-	sushi_router = '0xd9e1cE17f2641f24aE83637ab66a2cca9C378B9F'
-	dex_sushi = DexSwap(chain_id=42161,wallet_address=wallet_address,private_key=private_key,block_explorer_api=block_explorer_api,dex_exchange=sushi_router,base_trading_symbol='USDT')
-	print("dex_sushi ", dex_sushi)
-	#Execute ORDER to buy 1% of your USDT balance on SUSHISWAP ARBITRUM and get BTC token
-	demo_order = await dex_sushi.execute_order(direction = 'BUY',symbol = 'wBTC')
-	print("demo_order ", demo_order)
 ```
 ## Example
 [example](https://github.com/mraniki/dxsp/blob/main/examples/example.py)
 
 ## Real use case
 [TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
```

### Comparing `dxsp-2.0.9/dxsp/assets/blockchains.py` & `dxsp-2.1.0/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.9/dxsp/default_settings.toml` & `dxsp-2.1.0/dxsp/default_settings.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 [default]
 loglevel = "INFO"
 #📝tokenlist
+#headers = '{"User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.4 Safari/605.1.15"}'
+#headers = '{"accept": "application/json, text/plain, */*", "content-type": "application/json"}'
+#headers = '{"User-Agent": "Mozilla/5.0"}'
+headers = {User-Agent= 'Mozilla/5.0'}
+
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 #📝trading setup
 trading_quote_ccy = "USDT"
 trading_risk_amount = 10 # for 10% of the position
 trading_slippage = 2 #for 2 % slippage
@@ -14,15 +19,14 @@
 dex_block_explorer_api =  "798437294880920392"  #this is an example
 #chain_1 #see below for other chain ids or use https://chainlist.org to overwrite settings
 dex_chain_id = 1
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_block_explorer_url = "https://api.etherscan.io/api?"
 dex_protocol_type = "1inch" 
 dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D" 
-dex_base_api = "https://api.1inch.exchange/v5.0/1"
 
 #protocol specific
 #🦄1inch
 dex_1inch_url = "https://api.1inch.exchange/v5.0/"
 dex_1inch_limit_url = "https://limit-orders.1inch.io/v3.0/"
 #0️⃣0x
 dex_0x_url = "https://api.0x.org/mainnet/"
```

### Comparing `dxsp-2.0.9/dxsp/main.py` & `dxsp-2.1.0/dxsp/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,51 +48,61 @@
 
     async def _get(
         self,
         url,
         params=None,
         headers=None
             ):
-        headers = {"User-Agent": "Mozilla/5.0"}
-        response = requests.get(
-            url,
-            params=params,
-            headers=headers,
-            timeout=10)
-        return response.json()
+        try:
+            self.logger.debug("url: %s", url)
+            self.logger.debug("_header: %s", settings.headers)
+            response = requests.get(
+                url,
+                params=params,
+                headers={'User-Agent': 'Mozilla/5.0'},
+                timeout=10)
+            self.logger.error("_response: %s", response)
+            if response:
+                self.logger.debug("_json: %s", response.json())
+                return response.json()
+
+        except Exception as e:
+            self.logger.error("_get: %s", e)
 
     async def router(self):
         try:
             router_abi = await self.get_abi(settings.dex_router_contract_addr)
+            self.logger.debug("router_abi: %s", router_abi)
             router = self.w3.eth.contract(
                 self.w3.to_checksum_address(
                     settings.dex_router_contract_addr),
                 router_abi)
             return router
         except Exception as e:
             self.logger.error("router setup: %s", e)
-            return
 
     async def get_quote(
                 self,
                 symbol
             ):
-        self.logger.debug("get_quote %s", symbol)
+        self.logger.debug("get_quote")
         asset_in_address = await self.search_contract(symbol)
         asset_out_symbol = settings.trading_quote_ccy
         asset_out_address = await self.search_contract(asset_out_symbol)
         if asset_out_address is None:
-            self.logger.warning("No Valid Contract %s", symbol)
+            self.logger.warning("No Valid Contract")
             return
         try:
             if self.protocol_type in ["1inch", "1inch_limit"]:
+                self.logger.debug("1inch getquote")
                 await self.oneinch_quote(
                     asset_in_address,
                     asset_out_address)
             if self.protocol_type == "uniswap_v2":
+                self.logger.debug("uniswap_v2 getquote")
                 await self.uniswap_v2_quote(
                     asset_in_address,
                     asset_out_address)
             if self.protocol_type == "uniswap_v3":
                 await self.uniswap_v3_quote(
                     asset_in_address,
                     asset_out_address)
@@ -105,30 +115,34 @@
         asset_in_address,
         asset_out_address,
         amount=1
     ):
         try:
             asset_out_amount = self.w3.to_wei(amount, 'ether')
             quote_url = (
-                settings.dex_base_api
+                settings.dex_1inch_url
+                + "/"
+                + str(settings.chain_id)
                 + "/quote?fromTokenAddress="
                 + str(asset_in_address)
                 + "&toTokenAddress="
                 + str(asset_out_address)
                 + "&amount="
                 + str(asset_out_amount))
             quote_response = await self._get(quote_url)
-            quote_amount = quote_response['toTokenAmount']
-            # quote_decimals = quote_response['fromToken']['decimals']
-            quote = self.w3.from_wei(int(quote_amount), 'ether')
-            # /(10 ** quote_decimals))
-            return round(quote, 2)
+            self.logger.debug("quote_response %s", quote_response)
+            if quote_response:
+                quote_amount = quote_response['toTokenAmount']
+                self.logger.debug("quote_amount %s", quote_amount)
+                # quote_decimals = quote_response['fromToken']['decimals']
+                quote = self.w3.from_wei(int(quote_amount), 'ether')
+                # /(10 ** quote_decimals))
+                return round(quote, 2)
         except Exception as e:
             self.logger.error("oneinch_quote %s", e)
-            return
 
     async def uniswap_v2_quote(
         self,
         asset_in_address,
         asset_out_address,
         amount=1
     ):
@@ -279,26 +293,29 @@
 
     async def oneinch_swap(
         self,
         asset_out_address,
         asset_in_address,
         amount
     ):
-        swap_url = (settings.dex_base_api
-                    + "/swap?fromTokenAddress="
-                    + asset_out_address
-                    + "&toTokenAddress="
-                    + asset_in_address
-                    + "&amount="
-                    + amount
-                    + "&fromAddress="
-                    + self.wallet_address
-                    + "&slippage="
-                    + settings.trading_slippage
-                    )
+        swap_url = (
+            settings.dex_1inch_url
+            + "/"
+            + str(settings.chain_id)
+            + "/swap?fromTokenAddress="
+            + asset_out_address
+            + "&toTokenAddress="
+            + asset_in_address
+            + "&amount="
+            + amount
+            + "&fromAddress="
+            + self.wallet_address
+            + "&slippage="
+            + settings.trading_slippage
+            )
         swap_order = await self._get(swap_url)
         swap_order_status = swap_order['statusCode']
         if swap_order_status != 200:
             return
         return swap_order
 
     async def uniswap_v2_swap(
@@ -475,24 +492,28 @@
         except Exception as e:
             self.logger.error("get_approve %s", e)
             return None
 
     async def get_approve_1inch(self, asset_out_address):
         try:
             approval_check_URL = (
-                settings.dex_base_api
+                settings.dex_1inch_url
+                + "/"
+                + str(settings.chain_id)
                 + "/approve/allowance?tokenAddress="
                 + str(asset_out_address)
                 + "&walletAddress="
                 + str(self.wallet_address))
             approval_response = await self._get(approval_check_URL)
             approval_check = approval_response['allowance']
             if (approval_check == 0):
                 approval_URL = (
-                    settings.dex_base_api
+                    settings.dex_1inch_url
+                    + "/"
+                    + str(settings.chain_id)
                     + "/approve/transaction?tokenAddress="
                     + str(asset_out_address))
                 approval_response = await self._get(approval_URL)
                 return approval_response
         except Exception as e:
             self.logger.error("get_approve_uniswap %s", e)
             return None
@@ -618,15 +639,15 @@
 
     async def get_token_balance(
         self,
         token
          ):
 
         try:
-            token_contract = self.get_token_contract(token)
+            token_contract = await self.get_token_contract(token)
             token_balance = 0
             token_balance = token_contract.functions.balanceOf(
                 self.wallet_address).call()
             return 0 if token_balance <= 0 else token_balance
         except Exception as e:
             self.logger.error("get_token_balance: %s", e)
             return 0
```

### Comparing `dxsp-2.0.9/pyproject.toml` & `dxsp-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.0.9"
+version = "2.1.0"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-2.0.9/PKG-INFO` & `dxsp-2.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.0.9
+Version: 2.1.0
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -25,49 +25,39 @@
 | ------------- | ------------- |
 |[![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br>[![✨Flow](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH)](https://codecov.io/gh/mraniki/dxsp) <br>![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|24 blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>2 swap protocol (1inch API, UniV2 router)
 
 
 
 Key features:
 
-- 24 blockchains mainnet and testnet supported with default block explorer, RPC, Router (uniswap and pancakeswap) and protocol url (1inch and 0x). Other blockchains can be supported via function attributes
+- Any blockchains mainnet or testnet supported by web3py, 1inch or uniswap type router.
 - 2 swap protocol type supported:
 	- 1inch API v5
 	- Uniswap version 2 router protocol type
 
 Other features:
 - Translate token symbol to contract address via user defined tokenlist format or coingecko api 
-- Connect to web3  if no web3 object or no rpc provided
+- Connect to web3 if no web3 object or no rpc provided
 - Able to approve contract and sign transaction
 - Quote for a given token
 - Use Base symbol like stablecoin
-
+- Settings to use the modile for your own tool/bot
 
 
 # Install
 `pip install dxsp`
 
 # How to use it
 ```
 from dxsp import DexSwap
 
-	#SWAP HELPER
-	dex = DexSwap(chain_id=chain_id,wallet_address=wallet_address,private_key=private_key,block_explorer_api=block_explorer_api)
-	print("dex ", dex)
+	dex = DexSwap()
 	#BUY 10 USDC to SWAP with BITCOIN
 	demo_tx = await dex.get_swap('USDT','wBTC',10)
 	print("demo_tx ", demo_tx)
-
-	#SWAP with your OWN defined exchange like Sushiswap on ARBITRUM 
-	sushi_router = '0xd9e1cE17f2641f24aE83637ab66a2cca9C378B9F'
-	dex_sushi = DexSwap(chain_id=42161,wallet_address=wallet_address,private_key=private_key,block_explorer_api=block_explorer_api,dex_exchange=sushi_router,base_trading_symbol='USDT')
-	print("dex_sushi ", dex_sushi)
-	#Execute ORDER to buy 1% of your USDT balance on SUSHISWAP ARBITRUM and get BTC token
-	demo_order = await dex_sushi.execute_order(direction = 'BUY',symbol = 'wBTC')
-	print("demo_order ", demo_order)
 ```
 ## Example
 [example](https://github.com/mraniki/dxsp/blob/main/examples/example.py)
 
 ## Real use case
 [TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
```

